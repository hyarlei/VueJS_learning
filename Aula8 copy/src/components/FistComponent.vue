<template>
<div>
    <h1>Ola Vue!</h1>
    <p>meu nome eh {{nome}} e trabalho como {{profissao}}</p>
</div>
</template>

<script>
export default{
    name: 'FistComponent',
    data() {
        return{
            nome:'Thiago',
            profissao:'programador'
        }
    }
}
</script>