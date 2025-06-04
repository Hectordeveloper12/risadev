<script setup>

</script>

<template>
 <div class="imagem">
    <img src="../assets/img/img-inicio.svg" alt="">
 </div>

 <section class="inicio">
    <div class="lado-esquerdo">
        <div class="conteudo-p">
            <div class="titulo">
                <h1> <img src="../assets/img/seta-esquerda.svg" alt="<">
                Transformando<br> ideias em Soluções <br> Digitais de Impacto 
                <img src="../assets/img/seta-direita.svg" alt=">">
            </h1>
                
            </div>
            <div class="botoes">
            <a href=""><button class="btn-esquerdo">Serviços</button></a>
            <a href=""><button class="btn-direito">Contato</button></a>
                
            </div>
        </div>

        <div class="redes">
            <p>SIGA-NOS EM NOSSAS REDES</p>

            <div class="logo-redes">
                <a href=""><img src="../assets/img/instagram.svg" alt=""></a>
                <a href=""><img src="../assets/img/discord.svg" alt=""></a>
                <a href=""><img src="../assets/img/facebook.svg" alt=""></a>
                <a href=""><img src="../assets/img/X.svg" alt=""></a>
            </div>
        </div>
    </div>

    <div class="lado-direito">
        <img src="../assets/img/img-direita.svg" alt="">
    </div>
 </section>


</template>

<style scoped>
.imagem {
    img{
        position: absolute;
        bottom: -70px;
        width: 11%;
    }
}

.inicio {
    display: flex;
    justify-content: center;
    flex-direction: row;
    height: 91vh;
    margin-top: 150px;
    font-family: "Inter", sans-serif;

    .lado-esquerdo{
        z-index: 100;

        .conteudo-p {
            .titulo {
                margin-top: 72px;
                h1{
                    font-size: 4rem;
                    font-weight: 500;
                    color: var(--quinta-cor);
                    text-align: left;
                }
            }

            .botoes {
                    margin-top: 50px;        
                
                a{
                    text-decoration: none;    
                    margin: 0px 20px;        
                }

                .btn-esquerdo{
                background: var(--primeira-cor);
                height: 50px;
                width: 150px;
                border-radius: 50px;
                cursor: pointer;
                font-size: 16px; 
                border: none;
                color: var(--white);
                }
                .btn-direito{
                background: transparent;
                border: 1px solid var(--setima-cor);
                height: 50px;
                width: 150px;
                border-radius: 50px;
                cursor: pointer;
                font-size: 16px;
                color: var(--black);
            }
            }
        }

        .redes{
            display: flex;
            align-items: center;
            justify-content: center;
            flex-direction: column;
            position: relative; 
            top: 200px;
            left: -200px;

            p{
                margin-bottom: 15px;
                font-size: 12px;
                color: var(--setima-cor);
            }

            .logo-redes {
                img{
                    padding: 0px 5px;

                }
            }
        }
    }

    .lado-direito{

        img{
            position: relative;
            left: -22px;
            width: 100%;
        }
    }
}
</style>