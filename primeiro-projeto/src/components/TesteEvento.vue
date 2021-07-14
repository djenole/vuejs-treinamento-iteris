<template>
    <div class="teste-evento">
        <h3> Teste evento </h3>
        <p v-on:click="deixarMaiuscula">{{mensagem}}</p>
    </div>

</template>

<script>
export default {
    name:'TesteEvento',
    data() {
        return {
            
            mensagem:'Evento de click na frase'
        }
    },

    methods: {
        deixarMaiuscula() {
            this.mensagem = this.mensagem.toUpperCase();
        }
    }

}
</script>

<style scoped>

</style>