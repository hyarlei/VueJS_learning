<template>
  <div>
    <P v-if="esta_trabalhando">Estou trabalhando no momento</P>
    <p v-else>Estou em busca de novas oportunidades</p>
    <p>Utilizo essas tecnologias no meu dia dia</p>
    <ul>
      <li>javascript</li>
      <li>Nodejs</li>
      <li>React</li>
    </ul>
    <div>
      <button @click="showEmail"> {{text_bottom}}</button>
    </div>
    <p v-show="mostra_emails">Mande Uma mensagem para :{{ email }}</p>
    <p>
      Para acessa meu github
      <a v-bind:href="github">Clique aqui</a>
    </p>
    <Picture />
  </div>
</template>
<script lang="ts">
import Picture from "./Picture.vue";
export default {
  name: "Info",
  components: {
    Picture,
  },
  data() {
    return {
      esta_trabalhando: false,
      mostra_emails: false,
      email: "hyarleysf@gmail.com",
      github: "https://github.com/hyarlei",
      text_bottom:'mostra_emails'
    };
  },
  methods: {
    showEmail(){
      this.mostra_emails = !this.mostra_emails
      if(!this.mostra_emails){
        this.text_bottom = 'mostrar Email';
      }else{
        this.text_bottom = 'esconder Email';
      }

    }

  }

};
</script>