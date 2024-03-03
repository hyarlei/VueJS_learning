<template>
<div>
  <FistComponent/>
  <p>O dado de app é: {{teste}}</p>
</div>
</template>

<script>
import FistComponent from './components/FistComponent.vue'

export default{
    name:'App',
    components:{
        FistComponent
    },
    data(){
      return {
        teste:'testando'
      }
    }
}
</script>
