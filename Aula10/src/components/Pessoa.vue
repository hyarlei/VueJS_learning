<template>
  <div>
    <h2>Esta e a descricao de Pessoa: {{ nome }}</h2>
    <Info />
    <Form />
  </div>
</template>



<script>
import Form from "./Form.vue";
import Info from "./Info.vue";
export default {
  name: "Pessoa",
  components: {
    Info,
    Form,
  },
  data() {
    return {
      nome: "Hyarlei",
    };
  },
};
</script>