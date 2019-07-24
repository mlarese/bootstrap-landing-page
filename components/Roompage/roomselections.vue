<template>
  <!--eslint-disable-->
    <div class="container">
        <div class="row mt-5"><span style="color: #9E9D24"><h1>FIRST DEAL</h1></span></div>
        <div class="row mt-4"><span><h5>ROOM 1</h5></span></div>
        <div class="card row border-0 rounded-0" style="background-color: #ECEFF1">
                <div class="row">
                    <div class="col-4 col-sm-4 col-md-4 col-lg-4">
                        <img src="https://picsum.photos/510/301?random" class="img-fluid " alt="Responsive image" style="height: 100%">
                    </div>
                    <div class="col-8 col-sm-8 col-md-8 col-lg-8">
                        <div class=" row">
                            title

                        <span class="float-lg-right"><div>efcewfc</div></span></div>
                        <div class="row">fdcweewc</div>
                        <div class="row">
                            <p>{{ customer.reservation_paragraph }}</p>
                            <p>{{ customer.reservation_paragraph }}</p>
                        </div>
                    </div>
                </div>
        </div>
        <br>
        <div class="card row">
            <div class="card-header">
                <ul class="nav nav-tabs card-header-tabs">
                    <li class="nav-item">
                        <a class="nav-link active" href="#">Active</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Link</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link disabled" href="#">Disabled</a>
                    </li>
                </ul>
            </div>
            <div class="card-body">
                <h5 class="card-title">Special title treatment</h5>
                <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                <a href="#" class="btn btn-primary">Go somewhere</a>
            </div>
        </div>
        <br>
        <div class="row">
            <h3>TOTAL STAY</h3>
            <span class="ml-4">
                <h2>€ {{ booking.reservation_tot_reservation_price }} <sup> '00</sup>
                </h2>
            </span>
        </div>
        <div class="row align-baseline">
        <div class=" row col-10 col-sm-10 col-md-10 col-lg-10"> <h6>Confirmation deposit</h6>
            <span class="ml-4">
                <h6>€ {{ booking.reservation_tot_reservation_price }} <sup> '00</sup>
                </h6>
            </span>
        </div>
        <div class="row col-2 col-sm-2 col-md-2 col-lg-2 ml-lg-4">
            <button type="button"class="btn btn-outline-warning ml-5">
                Warning</button>
        </div>

        </div>
        <hr>
    </div>

</template>

<script>
    import {mapGetters} from 'vuex'
    export default {
        name: "Roomselections",
        computed: {
            ...mapGetters('reservation', ['booking','customer', 'room'])
        }
    }
</script>

<style scoped>

</style>
