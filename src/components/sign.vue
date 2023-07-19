<template>
    <div>
        <h1>{{ name }}</h1>
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

</style>