<template>
  <div class="chat">
    <div v-for="(msg, i) in mensagens" :key="i" :class="msg.tipo">
      <div class="balao">{{ msg.texto }}</div>
      <div v-if="msg.opcoes" class="opcoes">
        <button 
          v-for="(opt, j) in msg.opcoes" 
          :key="j" 
          @click="responder(opt)">
          {{ opt.texto }}
        </button>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const fluxo = {
  inicio: {
    tipo: 'bot',
    texto: 'Olá! Como posso ajudar?',
    opcoes: [
      { texto: 'Ver produtos', proxima: 'produtos' },
      { texto: 'Falar com suporte', proxima: 'suporte' }
    ]
  },
  produtos: {
    tipo: 'bot',
    texto: 'Temos os produtos A e B. Qual você quer?',
    opcoes: [
      { texto: 'Produto A', proxima: 'final' },
      { texto: 'Produto B', proxima: 'final' }
    ]
  },
  suporte: {
    tipo: 'bot',
    texto: 'Nosso suporte entrará em contato.',
    opcoes: []
  },
  final: {
    tipo: 'bot',
    texto: 'Obrigado pela escolha!',
    opcoes: []
  }
}

const mensagens = ref([
  fluxo['inicio']
])

function responder(opcao) {
  mensagens.value.push({
    tipo: 'usuario',
    texto: opcao.texto
  })

  const proxima = fluxo[opcao.proxima]
  if (proxima) mensagens.value.push(proxima)
}
</script>

<style scoped>
.chat {
  padding: 10px;
}
.bot {
  text-align: left;
}
.usuario {
  text-align: right;
}
.balao {
  display: inline-block;
  background: #eee;
  padding: 10px;
  border-radius: 10px;
  margin: 5px 0;
}
.opcoes {
  margin-top: 10px;
}
.opcoes button {
  margin-right: 5px;
}
</style>
