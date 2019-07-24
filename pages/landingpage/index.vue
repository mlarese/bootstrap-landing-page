<template>
  <div>
    <headers/>
    <welcomepage/>
    <br>
    <roomdetails/>
    <br>
    <roomselections/>
    <br>
    <footerdetails/>
  </div>
</template>
<script>
    import {mapState} from 'vuex'
    const root = {root: true}
    import headers from '../../components/Header/headers'
    import welcomepage from '../../components/Header/welcomepage'
    import roomdetails from '../../components/Roompage/roomdetails'
    import roomselections from '../../components/Roompage/roomselections'
    import footerdetails from '../../components/footer/footerdetails'
    export default {
        name: "IndexVue",
        components: {headers, welcomepage, roomdetails, roomselections, footerdetails},
        computed: {
            ...mapState('reservation', ['list']),

        },
        async fetch({store}) {
            await store.dispatch('reservation/load', {}, root)
        }
    }
</script>

<style scoped>

</style>
