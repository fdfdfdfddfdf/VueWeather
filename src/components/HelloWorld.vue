<template>
  <div class="informer-container">
    <Temperature v-bind:tempreal="temperatureReal" v-bind:tempfeel="temperatureFeel"/>
    <Flexbreak/>
    <Humidity v-bind:humidity="humidity"/>
    <Verticaldivider/>
    <Wind v-bind:wind="wind"/>
  </div>
</template>

<script>
import Temperature from './Temperature.vue'
import Humidity from './Humidity.vue'
import Wind from './Wind.vue'
import Flexbreak from './Flexbreak.vue'
import Verticaldivider from './Verticaldivider.vue'
export default{
  name: 'FirstComponent',
  components: {
    Temperature,
    Humidity,
    Wind,
    Flexbreak,
    Verticaldivider
  },
  data(){
    return {
      temperatureReal: 1,
      temperatureFeel: '-3.2',
      humidity: 6,
      wind: 20
    }
  }
}
</script>

<style>
.informer-container {
  display: flex;
  align-items: flex-start;
  justify-content: space-between;
  flex-wrap: wrap;
  width: 400px;
  min-height: 255px;
  padding: 30px;
  background-image: url('../img/forest.png');
  background-size: cover;
  background-position: center center;
  border-radius: 20px;
  box-shadow: 0px 0px 10px 0px rgba(50, 50, 50, 0.75);
}
</style>