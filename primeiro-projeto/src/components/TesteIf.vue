<template>
    <div class="teste-if"> 
        <h3 v-if="podeVer">Teste de invisibilidade</h3>
        <h3 v-else>Outro teste de invisibilidade </h3>
    </div>

</template>

<script>
export default {
    name: 'TesteIf',
    data() {
        return {
            podeVer: false
        }
    }
}
</script>

<style scoped>

</style>