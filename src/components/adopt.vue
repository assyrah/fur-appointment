<template>
    <b-container id="app-adopt" class="adopt-container d-flex" fluid>
        <b-container class="d-flex">
            <b-row align-v="center" align-h="center">
                <b-col cols="12" lg="8">
                    <h4>Adopting - 101</h4>
                    <p class="content">Class is in session! Here's a basic guide of what you would probably want to have
                        along with you at our adoption center:
                    </p>
                    <p class="content">
                        <ul>
                            <li>
                                <span class="pr-4">AN OPEN MIND</span>
                                Not all furry creatures are alike!
                            </li>
                            <li>
                                <span class="pr-4">COMFORTABLE SHOES</span>
                                You'll be on your feet all day, trust us!
                            </li>
                            <li>
                                <span class="pr-4">MOBILE PHONE</span>
                                To take pictures of your potential furry companion, of course!
                            </li>
                        </ul>
                    </p>
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
    .adopt-container {
        background-image: url("./../assets/bg_adopting101.jpg");
        background-size: cover;
        min-height: 35rem;
    }
    .content {
        color: $color-mono-400;
        font-size: $blue-light;
    }
    ul {
        padding-left: 0;
    }
    li {
        font-size: $font-size-base;
        span {
            font-family: $secondary-font;
            color: $orange;
            font-size: $font-size-lg;
        }
    }
</style>