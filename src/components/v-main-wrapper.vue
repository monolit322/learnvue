<template>
  <div class="v-main-wrapper">
    <p>{{title}}</p>
    <vCatalogVue/>
    <vCardVue/>
  </div>  
</template>

<script>
    import vCatalogVue from './v-catalog.vue';
    import vCardVue from './v-card.vue';

    export default{
        name: 'v-main-wrapper',
        components: {
            vCatalogVue,
            vCardVue,
        },
        props: {},
        data() {
            return {
                title: 'Main wrapper'
            }
        },
        computed: {},
        methods: {},
        watch: {},
        mounted() {
            console.log('Hellow i am alive')
        }
    }
</script>

<style>
    .v-main-wrapper{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        max-width: 900px;
        margin: 0 auto;
    }
</style>