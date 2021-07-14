<template>
    <div class="teste-for">
    <h4> Teste for </h4>

    <ul>
        <li v-for="objeto of objetos" v-bind:key="objeto.id">
            <img v-bind:src="objeto.url" v-bind:alt="objeto.nome">
        </li>

    </ul>
    </div>    
</template>

<script>
export default {
    name:"TesteFor",
    data() {
        return {
            objetos:[
                {
                    id: 1,
                    nome:'Jose',
                    url: 'https://scontent-gig2-1.xx.fbcdn.net/v/t1.6435-9/50221052_218839212279101_6141304931174318080_n.jpg?_nc_cat=108&ccb=1-3&_nc_sid=09cbfe&_nc_ohc=yWcXvskbOZUAX_H2I93&_nc_ht=scontent-gig2-1.xx&oh=bcf02aa6358fde5a0f6c770c8915e825&oe=60F323AC'

                },
                {
                    id:2,
                    nome:'Crianca',
                    url:'https://pbs.twimg.com/profile_images/1051517971892457473/Y8srRtA0_400x400.jpg'
                },
                {
                    id:3,
                    nome:'Gatinho',
                    url:'https://i.pinimg.com/280x280_RS/17/e8/f2/17e8f2cbde835840009c127364998b16.jpg'
                }
            ]

        }
    }
}
</script>

<style scoped>



</style>