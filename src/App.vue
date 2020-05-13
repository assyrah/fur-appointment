<template>
  <div id="app">
    <app-header></app-header>
    <app-countdown></app-countdown>
    <app-heroes></app-heroes>
    <app-meows></app-meows>
    <app-adopt></app-adopt>
    <app-appointment></app-appointment>
    <app-footer></app-footer>
  </div>
</template>

<script>
  import appHeader from './components/header.vue';
  import appFooter from './components/footer.vue';
  import appCountdown from './components/countdown.vue';
  import appHeroes from './components/heroes.vue';
  import appMeows from './components/meows.vue';
  import appAdopt from './components/adopt.vue';
  import appAppointment from './components/appointment.vue';

  export default {
    name: 'App',
    components: {
      'app-header': appHeader,
      'app-footer': appFooter,
      'app-countdown': appCountdown,
      'app-heroes': appHeroes,
      'app-meows': appMeows,
      'app-adopt': appAdopt,
      'app-appointment': appAppointment
    },
      data() {
        
      },
      created: function () {
        
      },
      methods: {
        
      }
  }
</script>

<style lang="scss">
  @import "./styles/main.scss"
</style>
