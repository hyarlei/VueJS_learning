<template>
<div>
    <h1>Olá Vue!</h1>
    <p>Meu nome é {{nome}} e trabalho com {{profissao}}</p>
</div>
</template>

<script>
export default{
    name: 'FistComponent',
    data() {
        return{
            nome:'Hyarlei',
            profissao:'Desenvolvimento Full Stack'
        }
    }
}
</script>