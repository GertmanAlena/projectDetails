<template>
    <div class="carousel">
        <div id="carouselExampleControls" class="carousel slide" data-ride="carousel">
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <img class="d-block w-100" src="../assets/image1.png" alt="Первый слайд">
                </div>
                <div class="carousel-item">
                    <img class="d-block w-100" src="../assets/Photo.png" alt="Второй слайд">
                </div>
                <div class="carousel-item">
                    <img class="d-block w-100" src="../assets/image2.png" alt="Третий слайд">
                </div>
            </div>
            <a class="carousel-control-prev" href="#carouselExampleControls" role="button" data-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="sr-only">Previous</span>
            </a>
            <a class="carousel-control-next" href="#carouselExampleControls" role="button" data-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="sr-only">Next</span>
            </a>
        </div>
    </div>

</template>

<script>

export default {
    name: 'CarouselComponent',

    data() {
        return {

        };
    },

    mounted() {

    },

    methods: {

    },
};
</script>
<style>
    .carousel {
        padding-left: calc(50% - 1200px/2);
        padding-right: calc(50% - 1200px/2);
    }
    .d-block{
        border-radius: 100px 100px 100px 100px;
    }
</style>