<template>
  <div>
    <FistComponent />
    <p>O dado de app é: {{ teste }}</p>
    <LifeCycle />
    <Pessoa />
  </div>
</template>

<script>
import FistComponent from "./components/FistComponent.vue";
import LifeCycle from "./components/LifeCycle.vue";
import Pessoa from "./components/Pessoa.vue";

export default {
  name: "App",
  components: {
    FistComponent,
    LifeCycle,
    Pessoa,
  },
  data() {
    return {
      teste: "testando",
    };
  },
};
</script>
