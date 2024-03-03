<template>
    <h1>Ola Vue!,ola:{{nome}}</h1>
    
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
        this.nome="Hyarlei"
    },1000)
     
    },
    mounted(){
    setTimeout(() =>{
        this.nome="Felipe"
    },2000)
       
    }
}
</script>