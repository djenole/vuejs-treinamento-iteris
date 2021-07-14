<template>
    <div class="clubes-futebol">
        <h3>consumindo API</h3>
        <ul>
            <li v-for="site of sites" :key="site.id">
                <a :href="site.link" >{{site.nome}} - {{site.pontos}}</a>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'ClubesFutebol',
    data() {
        return {
            sites: []
        }
    },

    created() {
        fetch('https://hackthon-decola.firebaseio.com/clubes-lista.json')
            .then(resultado => resultado.json())
            .then(json => {
                this.sites = json;
            })
    }
}
</script>

<style scoped>

</style>