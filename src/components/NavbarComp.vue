<script setup>

</script>

<template>
    <nav class="navbar">
        <div class="logo">
            <img src="../assets/img/LOGO.svg" alt="">
        </div>

        <div class="menu">
            <ul>
                <li><a href="">Serviços</a></li>
                <li><a href="">Hospedagem</a></li>
                <li><a href="">Depoimentos</a></li>
                <li><a href="">Desenvolvimento</a></li>
            </ul>
        </div>
        
        <div class="botao">
            <a href=""><button>Contato</button></a>
        </div>
    </nav>
</template>

<style scoped>
.navbar {
    display: flex;
    align-items: center;
    justify-content: space-around;
    width: 100%;
    height: 100px;
    font-family: "Inter", sans-serif;
    .menu{
        ul{
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: row;

        li{
            list-style: none;

            a{
                text-decoration: none;
                color: var(--black);
                padding: 0px 30px;
                font-size: 16px;
            }
        }
        }
    }

    .botao {
            a{
                    text-decoration: none;
                    color: var(--black);
                    

                button{
                background: transparent;
                border: 1px solid var(--setima-cor);
                height: 50px;
                width: 150px;
                border-radius: 50px;
                cursor: pointer;
                font-size: 16px;

            }
                }

    }

}

</style>