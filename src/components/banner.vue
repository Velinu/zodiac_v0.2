<template>
    <div id="banner-container">
        <h1>Mergulhe no universo<br/> dos astros</h1>
        <button>Descubra sobre os signos</button>
    </div>
</template>

<script>

    export default {
        name: "mainBanner",
        props: {
            alt: String
        }
    }

</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');
#banner-container{
        padding-top: 28vh;
        letter-spacing: 5px;
        background-image: url("https://images.contentstack.io/v3/assets/blt187521ff0727be24/bltfa2ed957e2b1ac7c/60ee0fa4eebf8245e1b490f1/mttargon-once-in-a-lifetime.jpg");
        padding-bottom: 35.3vh;
        display: flex;
        flex-direction: column;
        align-items: end;
        padding-right: 10vw;
    }

#banner-container h1{
    color: #FFDD33;
    font-size: 2.8em;
}

#banner-container button{
    width: 31vw;
    height: 10vh;
    font-family: 'Montserrat', sans-serif;
    font-size: 1.2em;
    letter-spacing: 0.5px;
    background-color: transparent;
    border: 4px solid #FFDD33;
    color: #FFDD33;
    transition: 0.1s ease-in;
}

#banner-container button:hover{
    cursor: pointer;
    background-color: #FFDD33;
    color: black;
    font-weight: bolder;
}

</style>