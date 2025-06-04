<script setup>

</script>

<template>
    <section class="servicos">
        <div class="subtitulo">
            <h2>Serviços</h2>
        </div>

        <div class="titulo">
            <h1>Soluções que se encaixam na sua necessidade</h1>
        </div>

        <div class="cards">

            <div class="cardmain">

            <div class="card">
                <div class="img">
                    <img src="../assets/img/Web.svg" alt="">
                </div>

                <a href="">Desenvolvimento Web <img src="../assets/img/arrow.svg" alt=""></a>
                <div class="paragrafo">
                    <p>Transforme sua presença online com nossas soluções completas de desenvolvimento web.</p>
                </div>
            </div>

            <div class="card">
                <div class="img">
                    <img src="../assets/img/UI UX.svg" alt="">
                </div>
                <a href="">Design e UX <img src="../assets/img/arrow.svg" alt=""></a>
                <div class="paragrafo">
                    <p>Cative seu público com designs visualmente deslumbrantes e centrados no usuário.</p>
                </div>
            </div>

            <div class="card">
                <div class="img">
                    <img src="../assets/img/HOSPEDAGEM.svg" alt="">
                </div>
                <a href="">Hospedagem de Sites <img src="../assets/img/arrow.svg" alt=""></a>
                <div class="paragrafo">
                    <p>Hospede seu site com segurança e performance em nossos servidores otimizados.</p>
                </div>
            </div>

            </div>
           
            <div class="cardmain">

            <div class="card">
                <div class="img">
                    <img src="../assets/img/BOT.svg" alt="">
                </div>

                <a href="">Bots de texto <img src="../assets/img/arrow.svg" alt=""></a>
                <div class="paragrafo">
                    <p>Automatize e otimize a comunicação com bots personalizados</p>
                </div>
            </div>

            <div class="card">
                <div class="img">
                    <img src="../assets/img/JOGOS.svg" alt="">
                </div>
                <a href="">Servidores em Jogos <img src="../assets/img/arrow.svg" alt=""></a>
                <div class="paragrafo">
                    <p>Crie servidores rápidos e ótimizados para seus jogos favoritos.</p>
                </div>
            </div>

            <div class="card">
                <div class="img">
                    <img src="../assets/img/CLOUD.svg" alt="">
                </div>

                <a href="">Servidor Cloud <img src="../assets/img/arrow.svg" alt=""></a>
                <div class="paragrafo">
                    <p>Tenha o poder e a flexibilidade de servidores VPS de alta performance para suas necessidades específicas.</p>
                </div>
            </div>

            </div>

        </div>
    </section>
</template>

<style scoped>
.servicos {
    display: flex;
    align-items: center;
    justify-content: start;
    flex-direction: column;
    font-family: "Inter", sans-serif;
    width: 100%;
    height: 50vh;
    .subtitulo{
        display: flex;
        align-items: start;
        width: 100%;
        margin-bottom: 10px;
        padding-left: 11.3%;
        color: var(--setima-cor);
        font-weight: 100;
    }
    .titulo{
        display: flex;
        align-items: start;
        width: 100%;
        padding-left: 11.3%;
    }


    .cards {
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        width: 100%;
        .cardmain{
            width: 100%;
            display: flex;
            align-items: center;
            justify-content: space-evenly;
            flex-direction: row;
        .card{
            height: 185px;
            width: 346px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: start;

            a{
                font-size: 24px;
                color: var(--primeira-cor);
                text-decoration: none;
                font-weight: bold;
                border-bottom: 1px solid var(--primeira-cor);
                
                img{
                    margin-left: 5px;
                }
            }

            .img{
                height: 50px;
                width: 50px;

                img{
                    position: absolute;
                }
            }
            
        }
        }

        .paragrafo{

            p{  
                margin-top: 5px;
                width: 400px;
                position: absolute;
            }
        }
    }
    
}
</style>