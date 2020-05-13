<template>
    <b-container id="app-countdown" class="countdown-container d-flex" fluid>
        <b-container class="d-flex">
            <b-row align-v="center">
                <b-col md="8" sm="auto">
                    <h1>LAST CHANCE TO ADOPT!</h1>
                    <p class="countdown">{{hours}} hours {{minutes}} mins left</p>
                    <a class="button" href="#app-appointment">MAKE APPOINTMENT NOW</a>
                </b-col>
            </b-row>
        </b-container>
    </b-container>
</template>

<script>
    export default {
        data: function(){
            return{
                interval: "",
                minutes:"",
                hours:""
            }
        },
        mounted(){
            var timeLeft = new Date();
            timeLeft.setHours(timeLeft.getHours() + 4);
            timeLeft.setMinutes(timeLeft.getMinutes() + 30);
            this.timerCount(timeLeft);
            this.interval = setInterval(() => {
                this.timerCount(timeLeft);
            }, 1000);
        },
        methods: {
            timerCount: function(timeLeft){
                var now = new Date().getTime();
                var passTime =  timeLeft - now;

                if(passTime < 0){
                    clearInterval(this.interval);
                    return;

                }else if(passTime > 0){
                    this.calcTime(passTime);
                }
            },
            calcTime: function(dist){
                this.hours = Math.floor((dist % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
                this.minutes = Math.floor((dist % (1000 * 60 * 60)) / (1000 * 60));
            }
            
        }
        }
</script>

<style lang=scss scoped>
    .countdown-container {
        background-image: url("./../assets/bg_header1.jpg");
        background-size: cover;
        min-height: 48rem;
    }
    .countdown {
        color: $color-font-inverted;
        font-size: $font-size-lg;
    }
</style>