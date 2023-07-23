<template>
  <navBar />
  <mainBanner />
  
  <bannerSigns />
  <div v-for="sign in signs" :key="sign.id">
    <signsComp 
    :name="sign.nome" 
    :description="sign.descricao" 
    :date="sign.datas_de_nascimento"
    :img="sign.imagem"/>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import navBar from './components/navBar.vue'
import mainBanner from './components/banner.vue'
import signsComp from './components/sign.vue'
import bannerSigns from './components/bannerSigns.vue'
export default defineComponent({
  name: 'App',
  components: {
    navBar,
    mainBanner,
    signsComp,
    bannerSigns
  },
  data() {
    return{
      signs: null
    }
  },
  methods: {
    async getSignInfo(){
      const req = await fetch("http://localhost:3000/signos");
      const data = await req.json();
      this.signs = data
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
