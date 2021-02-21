<template>
  <div id="app">
    <h1>Conversor de Moedas</h1>
    <h3>Principais Moedas Estrangeiras x Real (BRL)</h3>
    <div class="linha">
    <conversor moeda-a="USD" moeda-b="BRL"/>
    <conversor moeda-a="CAD" moeda-b="BRL"/>
    <conversor moeda-a="ARS" moeda-b="BRL"/>
  </div>
  <div class="linha">
    <conversor moeda-a="EUR" moeda-b="BRL"/>
    <conversor moeda-a="GBP" moeda-b="BRL"/>
    <conversor moeda-a="MXN" moeda-b="BRL"/>
    
    </div>
    <h3>Real  (BRL) x Moedas estrangeiras</h3>
    <div class="linha">
    <conversor moeda-a="BRL" moeda-b="USD"/>
    <conversor moeda-a="BRL" moeda-b="EUR"/>
    <conversor moeda-a="BRL" moeda-b="GBP"/>
    </div>
  </div>
</template>

<script>
import conversor from "./components/conversor";
export default {
  name: 'App',
  components: {
    conversor
  }
};
</script>

<style>
#app {
  margin: auto;
  max-width: 900px;
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.linha{
    margin-top: 40px;
    display: flex;
    justify-content: space-between;
}
</style>
