<template>
    <b-container id="app-meows" class="meows-container d-flex" fluid>
        <b-container class="d-flex">
            <b-row align-v="center">
                <b-col cols="12" lg="6" sm="auto">
                    <h3>Hall of meows.</h3>
                    <p class="meows">Featured felines of the week!</p>
                    <b-row align-h="center" class="text-center">
                        <b-col cols="6" lg="4">
                            <b-img src="./../assets/gallery_01.png" class="logo navbar-item mb-4"></b-img>
                        </b-col>
                        <b-col cols="6" lg="4">
                            <b-img src="./../assets/gallery_02.png" class="logo navbar-item mb-4"></b-img>
                        </b-col>
                        <b-col cols="6" lg="4">
                            <b-img src="./../assets/gallery_03.png" class="logo navbar-item mb-4"></b-img>
                        </b-col>
                        <b-col cols="6" lg="4">
                            <b-img src="./../assets/gallery_04.png" class="logo navbar-item mb-4"></b-img>
                        </b-col>
                        <b-col cols="6" lg="4">
                            <b-img src="./../assets/gallery_05.png" class="logo navbar-item mb-4"></b-img>
                        </b-col>
                        <b-col cols="6" lg="4">
                            <b-img src="./../assets/gallery_06.png" class="logo navbar-item mb-4"></b-img>
                        </b-col>
                    </b-row>
                    <a class="button" href="#">BROWSE NOW</a>
                </b-col>
            </b-row>
        </b-container>
    </b-container>
</template>

<script>
    export default {
        
    }
</script>

<style lang=scss scoped>
    .meows-container {
        background-image: url("./../assets/bg_hallofmeows.jpg");
        background-size: cover;
        min-height: 48rem;
    }
    .meows {
        color: $blue;
        font-weight: 600;
        font-size: $font-size-lg;
    }
    img {
        border: 3px solid $color-mono-100;
    }
</style>