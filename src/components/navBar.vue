<template>
    <header>
        <div id="title">
            <img src="/assets/icons/astrology.png" alt="icon"/>
            <h1>Zodiac</h1>
        </div>

        <div id="buttons-container">
            <button class="nav-buttom">Meu Signo</button>
            <button class="nav-buttom">Sobre os Signos</button>
        </div>

    </header>
</template>

<script>
    export default{
        name: "navBar"
    }
</script>

<style>
    header{
        display: flex;
        align-items: center;
        position: relative;
        justify-content: end;
        height: 10vh;
        color: #001F6D;
        box-shadow: 0 0 20px rgba(0, 0, 0, 0.242);
    }

    #title{
        user-select: none;
        margin-right:53vw;
        font-size: 1.2em;
        display: flex;
        align-items: center;
    }

    #title img{
        width: 3vw;
        height: 6vh;
        margin-right: 1vw;
    }

    #buttons-container{
        margin-right: 10vw;
        font-size: 2em;
    }

    .nav-buttom{
        padding: 4vh 1.5vw;
        color: #001F6D;
        background-color: transparent;
        border: none;
        font-size: 0.6em;
        text-shadow: rgb(252, 252, 252) 1px 0px 5px;
        cursor: pointer;
        position: relative;
    }

    .nav-buttom::after{
        content: '';
        width: 100%;
        height: 0%;
        left: 0%;
        bottom: 0;
        position: absolute;
        background-color: #001f6d;
        transition: 0.2s ease-in-out;
        z-index: -1;
    }
    .nav-buttom:hover{
        color: white;
        text-shadow: rgb(252, 252, 252) 1px 0px 10px;
    }
    .nav-buttom:hover:after{
        width: 100%;
        height: 100%;
    }


</style>