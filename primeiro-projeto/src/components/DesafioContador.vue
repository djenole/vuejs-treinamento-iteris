<template>
    <div class="desafio-contador">

        <h3>Contador:{{contador}}</h3>

        <button v-on:click="incrementar()">+</button>
        <button v-on:click="decrementar()">-</button>
      
    </div>
</template>
    
<script>
export default {
    name: 'DesafioContador',
    data() {
        return {
            contador: 0
        }
    },

    methods: {
        incrementar() {
            return this.contador++;
        },
        decrementar() {
            return this.contador--;
        }
    }
   
    
}
</script>

<style scoped>

</style>