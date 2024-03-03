<template>
<div>
  <FistComponent/>
  <p>O dado de app é: {{teste}}</p>
  <LifeCycle/>
</div>
</template>

<script>
import FistComponent from './components/FistComponent.vue'
import LifeCycle from './components/LifeCycle.vue'

export default{
    name:'App',
    components:{
        FistComponent,
        LifeCycle
    },
    data(){
      return {
        teste:'testando'
      }
    }
}
</script>
