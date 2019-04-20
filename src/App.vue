<template>
  <div id="app">
    <h1>Conversor de Moedas</h1>
    <div class="linha">
      <Conversor moeda-a="USD" moeda-b="BRL"/>
      <Conversor moeda-a="BRL" moeda-b="USD"/>
    </div>
    <div class="linha">
      <Conversor moeda-a="EUR" moeda-b="BRL"/>
      <Conversor moeda-a="BRL" moeda-b="EUR"/>
    </div>
  </div>
</template>

<script>
import Conversor from "./components/Conversor.vue";
export default {
  name: 'app',
  components: {
    Conversor
  }
};
</script>

<style>
#app {
  max-width: 900px;
  margin:auto;
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.linha{
  margin-top:40px;
  display: flex;
  justify-content: space-around;
}
</style>
