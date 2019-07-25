<template>
  <!--eslint-disable-->
    <div>
    <div style="text-align: center"><h6>Hotel Ambassador C 2017</h6></div>
    <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
        <div class="carousel-inner" style="height: 700px">
            <div class="carousel-item active">
                <img src="https://picsum.photos/510/303?random" alt="Chicago" style="width:100%;">
            </div>
            <div class="carousel-item">
                <img src="https://picsum.photos/510/302?random" alt="Chicago" style="width:100%;">
            </div>
            <div class="carousel-item">
                <img src="https://picsum.photos/510/301?random" alt="Chicago" style="width:100%;">
            </div>
        </div>
        <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="sr-only">Previous</span>
        </a>
        <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="sr-only">Next</span>
        </a>
        <div class="carousel-caption d-none d-md-block">
            <span>Look through our page</span>
            <h1>For the best offers</h1>
            <div class="dropup"><icon>arrow</icon></div>
        </div>
    </div>
    </div>
</template>

<script>
    export default {
        name: "Headers"
    }
</script>

<style scoped>

</style>
