<template>
  <navBar />
  <mainBanner />
  
  <signsComp name=""/>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import navBar from './components/navBar.vue'
import mainBanner from './components/banner.vue'
import signsComp from './components/sign.vue'
export default defineComponent({
  name: 'App',
  components: {
    navBar,
    mainBanner,
    signsComp
  },
  methods: {
    async getSignInfo(){
      const req = await fetch("http://localhost:3000/signos");
      const data = await req.json();

      console.log(data)
    }
  },
  mounted() {
    this.getSignInfo()
  }
});
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');
body{
  margin: 0;
  font-family: 'Montserrat', sans-serif;
  letter-spacing: 5px;
}



</style>
