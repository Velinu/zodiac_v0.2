<template>
    <div id="banner-container" :image="url( )">
        <img :src="banner" :alt="alt" />
    </div>
</template>

<script>

    export default {
        name: "bannerTemplate",
        props: {
            banner: String,
            alt: String
        }
    }

</script>

<style>

</style>