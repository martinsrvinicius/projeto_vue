<template>
  <h1>Meu nome é {{ nome }}</h1>
  <Info />
</template>

<script>

import Info from './Info.vue'
export default {
  name: 'LifeCycle',
  components: {
    Info
  },
  data() {
    return { 
      nome: "Ainda não sei"
    }
  },
  created() {
    setTimeout(() => {
        this.nome = 'Matheus'   
        this.LifeCycle() 
    }, 1000);
  },
  mounted(){
    setTimeout(() => {
        this.nome = 'Vinicius'
        this.LifeCycle();
    }, 2000);
  },
  methods: {
    LifeCycle(){
      console.log(`Executou`);
    }
  }
}
</script>