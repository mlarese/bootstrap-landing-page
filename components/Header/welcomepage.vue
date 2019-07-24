<template>
  <div class="container">
    <br>
    <div
      class="text-md-center"
    >
      <div
        class="title"
        style="color: #9E9D24">
        <span class="title">Good morning{{ customer.reservation_name }} {{ customer.reservation_surname }}</span>
      </div>
    </div>
    <div
      class="pt-3 text-center"
    >
      <p> {{ customer.reservation_paragraph }} </p>
      <p> {{ customer.reservation_paragraph }} </p>
      <p> {{ customer.reservation_paragraph }} </p>
    </div>
    <div class="px-3">
      <em><small>The Staff of Hotel Ambassador </small></em>
    </div>
  </div>
</template>

<script>
    import {mapGetters} from 'vuex'
    export default {
        name: "Welcomepage",
        computed: {
            ...mapGetters('reservation', ['customer'])
        }
    }
</script>

<style scoped>

</style>
