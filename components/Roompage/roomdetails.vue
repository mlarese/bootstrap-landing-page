<template>
  <!--eslint-disable-->
    <div class="card container align-content-center border-0 rounded-0" style="background-color: #ECEFF1">
      <div class="card-body" >
        <h4 class="card-title" style="color: #9E9D24"> SUMMARY OF YOUR REQUEST</h4>
          <div class="row">
              <div class="col-6 col-sm-6 col-md-6 col-lg-3"><input size="20" type="date" disabled value="12-02-2012" readonly></div>
              <div class="col-6 col-sm-6 col-md-6 col-lg-3"><input size="20" type="date" disabled value="12-02-2012" readonly></div>
              <div class="col-6 col-xs-6 col-sm-6 col-md-6 col-lg-3"><input size="20" type="number" disabled value="12-02-2012" readonly></div>
              <div class="col-6 col-sm-6 col-md-6 col-lg-3"><input size="20" type="number" disabled value="12-02-2012" readonly></div>
          </div>
          <br><br>
          <div><span class="card-subtitle">CARRY OUT BY</span></div>
          <div class="row">
              <div class="col-6 col-sm-6 col-md-6 col-lg-3"><span> Name:</span> <strong>{{ customer.reservation_name }}</strong></div>
              <div class="col-6 col-sm-6 col-md-6 col-lg-3"><span> Surname:</span> <strong>{{ customer.reservation_surname }}</strong></div>
              <div class="col-6 col-sm-6 col-md-6 col-lg-3"><span> Phone Number:</span> <strong>{{ customer.reservation_phone }}</strong></div>
              <div class="col-6 col-sm-6 col-md-6 col-lg-3"><small><span> E-mail:</span> <strong>{{ customer.reservation_email }}</strong></small></div>
          </div>
          <div class="row mt-3">
              <div class="col-6 col-sm-6 col-md-6 col-lg-3"><span> Address:</span> <strong>{{ customer.reservation_address }}</strong></div>
              <div class="col-6 col-sm-6 col-md-6 col-lg-3"><span> City:</span> <strong>{{ customer.reservation_city }}</strong></div>
              <div class="col-6 col-sm-6 col-md-6 col-lg-3"><span> Province:</span> <strong>{{ customer.reservation_state }}</strong></div>
          </div>
          <div class="row mb-2 mt-3">
              <div class="col-6 col-sm-6 col-md-6 col-lg-6"><strong>EXPIRY PREVENTIVE</strong></div>
              <div class="col-6 col-sm-6 col-md-6 col-lg-6"><span>PROTOCOL</span></div>
          </div>
          <div class="row mb-3">
              <div class="col-6 col-sm-6 col-md-6 col-lg-6"><span class="text-danger"> Expire:</span> <strong class="text-danger">{{ customer.reservation_expiration_date }}</strong></div>
              <div class="col-6 col-sm-6 col-md-6 col-lg-6"><span> Protocol Number:</span> <strong>{{ customer.reservation_remote_address }}</strong></div>
          </div>
      </div>

    </div>
</template>

<script>
    import {mapGetters} from 'vuex'
    export default {
        name: "Roomdetails",
        computed: {
            ...mapGetters('reservation', ['booking', 'customer'])
        }
    }
</script>

<style scoped>

</style>
