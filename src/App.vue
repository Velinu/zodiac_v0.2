<template>
  <navBar />
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import navBar from './components/navBar.vue'
export default defineComponent({
  name: 'App',
  components: {
    navBar
  }
});
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');
body{
  margin: 0;
  font-family: 'Montserrat', sans-serif;
}

</style>
