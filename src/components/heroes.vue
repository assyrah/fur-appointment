<template>
    <b-container id="app-heroes" class="heroes-container text-center mt-5 mb-5 container">
            <b-row align-v="center" align-h="center">
                <b-col cols="12" lg="9">
                    <h2>Only heroes - adopt.</h2>
                    <p class="content"><strong>Not all heroes wear capes!</strong> Saving the world is not a job that is only exclusive 
                        to comic heroes in new york city...<br>
                        Now, you can do your part with one paw at a time.
                    </p>
                </b-col>
            </b-row>
        <b-row align-h="center">
            <b-col cols="12" lg="3">
                <b-img src="./../assets/graphic_01.png" class="logo navbar-item mb-4"></b-img>
                <h5>TRUE COMPANIONSHIP</h5>
                <p><small>Opening your doors to your new furry friend brings a wholesome new meaning to friendship.</small></p>
            </b-col>
            <b-col cols="12" lg="3">
                <b-img src="./../assets/graphic_02.png" class="logo navbar-item mb-4"></b-img>
                <h5>FULFILLING ROLE</h5>
                <p><small>The major side effect of being there for your furry friend is feeling rewarded when they purr!</small></p>
            </b-col>
            <b-col cols="12" lg="3">
                <b-img src="./../assets/graphic_03.png" class="logo navbar-item mb-4"></b-img>
                <h5>LOVING COMMUNITY</h5>
                <p><small>You will be part of huge and growing community of adopters, worldwide, to share your experiences!</small></p>
            </b-col>
        </b-row>
    </b-container>
</template>

<script>
    export default {
        
    }
</script>

<style lang=scss scoped>
    .content {
        font-size: $font-size-lg;
    }
</style>