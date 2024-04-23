<template>
  <div id="app">
    <h1>Chuck Norris Jokes</h1>
    <div class="container">
      <div class="row">
        <chuck-card v-for="(joke, index) in chuck" :key="index" :icon-url="joke.icon_url" :value="joke.value"></chuck-card>
      </div>
    </div>
  </div>
</template>

<script>
import ChuckCard from './components/ChuckCard.vue';

export default {
  components: {
    ChuckCard
  },
  data() {
    return {
      chuck: [
        { "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", "value": "Chuck Norris can skydive into outer space." },
        { "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", "value": "The chief export of Chuck Norris is pain." },
        { "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", "value": "Chuck Norris doesn't read books. He stares them down until he gets the information he wants." },
        { "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", "value": "Time waits for no man. Unless that man is Chuck Norris." },
        { "icon_url": "https://assets.chucknorris.host/img/avatar/chuck-norris.png", "value": "If you spell Chuck Norris in Scrabble, you win. Forever." },
      ]
    }
  }
}
</script>

<style scoped>
#app {
  text-align: center;
}

h1 {
  background-color: #333;
  color: #fff;
  padding: 20px;
}

.container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  margin-top: 20px;
}

.row {
  margin-bottom: 20px;
}

/* Estilos para cada tarjeta */
.chuck-card {
  width: 300px;
  margin-right: 20px;
  margin-bottom: 20px;
}

.card-img-top {
  max-width: 100%;
}

.card-text {
  margin-top: 10px;
}
</style>
