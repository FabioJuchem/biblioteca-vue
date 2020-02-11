<template>
  <div id="app">
  <router-view></router-view>
    <div class="teste">
      <biblioteca :texto="'Igor baiano'"/>
    </div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import biblioteca from 'biblioteca';

@Component({
  components: {
    biblioteca,
  },
})
export default class App extends Vue {}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.teste {
  border: 2px solid black
}
</style>
