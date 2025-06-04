<script setup>

</script>

<template>
    <section class="cloud">
        <div class="lado-esquerdo">
            <h2>Servidores Cloud</h2>
            <h1>Escalabilidade e Desempenho na Nuvem</h1>
            <p>Garanta a melhor experiência para seus projetos com nossa infraestrutura robusta e escalável, pronta para atender às demandas mais exigentes.</p>
           <a href=""><button>Saiba mais</button></a> 
        </div>

        <div class="lado-direito">
            <img src="../assets/img/CLOUDIMG.svg" alt="logo">
        </div>

    </section>
</template>

<style scoped>
.cloud{
    width: 100%;
    height: 55vh;
    display: flex;
    align-items: start;
    justify-content: start;
    font-family: "Inter", sans-serif;
    padding-left: 11%;

    .lado-esquerdo{

        h2{
            color: var(--setima-cor);
            font-weight: 500;
            margin-bottom: 30px;
            margin-top: 150px;
        }
        h1{
                    font-size: 36px;
                    font-weight: 500;
                    margin-bottom: 50px;

        }

        p{
            width: 500px;
            font-size: 16px;
            margin-bottom: 40px;
        }

        a{
                    text-decoration: none;        
                    
                    button{
                background: var(--primeira-cor);
                height: 50px;
                width: 150px;
                border-radius: 50px;
                cursor: pointer;
                font-size: 16px; 
                border: none;
                color: var(--white);
                    }
                }

        

        
    }

    .lado-direito{
        img{
            position: absolute;
            right: 0px;
        }
    }
}
</style>