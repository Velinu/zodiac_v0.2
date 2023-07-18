<template>
    <div>
        <h1>{{ name }}</h1>
    </div>
</template>

<script>
    export default {
        name: "signsComp",
        props: {
            id: Number,
            name: String,
            img: String,
            date: String
        },
        methods: {
            async getInfo() {
                const req = await fetch("")
            }
        }
    }

</script>

<style>

</style>