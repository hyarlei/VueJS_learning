<template>
    <h1>Ola Vue! ola:{{nome}}</h1>
    
</template>

<script>
export default {
    name:'LyfeCycles',
    data(){
        return {
        nome:'Ainda nao sei'
        }
    },
    created(){
    setTimeout(() =>{
        this.nome="Thiago"
      this.executou();
    },1000)
     
    },
    mounted(){
    setTimeout(() =>{
        this.nome="Thiago"
      this.executou();
    },2000)
       
    },
  methods:{
      executou(){
        console.log("executou")
      }

  }
}
</script>