<template>
  <div id="app">
    <div class="upper-bar">
      <img src="./assets/icons/minimize.svg" alt="-" @mousedown="clickHold()" />
      <img src="./assets/icons/Resize.svg" alt />
      <img src="./assets/icons/quit.svg" alt />
    </div>
    <h1>Hello World</h1>
  </div>
</template>
<script lang="ts">
import Vue from "vue";
export default Vue.extend({});
</script>
<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.upper-bar {
  display: flex;
  justify-content: flex-end;
  img {
    height: 15px;
    width: 15px;
    padding: 0 2px;
  }
  img:hover {
    cursor: pointer;
    filter: invert(0.6) sepia(0.5);
  }
  img:active {
    scale: 0.5;
  }
}
</style>
