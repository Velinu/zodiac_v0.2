<template>
    <div id="sign-container">
        <h1>{{ name }}</h1>
        <img :src="img" :alt="name">
        <h2>Datas de nascimento</h2>
        <h2>{{ date }}</h2>
    </div>
</template>

<script>
    export default {
        name: "signsComp",
        props: {
            id: null,
            name: null,
            img: null,
            date: null,
            description: null
        },
        methods: {
            
        }
    }

</script>

<style>
    #sign-container{
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    img{
        width: 10vw;
        height: 14vh;
    }
</style>