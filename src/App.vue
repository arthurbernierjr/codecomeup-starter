<template>
  <div id="app">
      <img id="logo" alt="Vue logo" src="./assets/logo.png">
    <LayoutHeader/>
  </div>
</template>

<script>
import LayoutHeader from './components/LayoutHeader'
export default {
  name: 'app',
  components: {
    LayoutHeader
  }
}
</script>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  #logo{
    height: 20vw;
    width: 25vw;
    animation: rotation 2s infinite linear;
  }
  @keyframes rotation {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(359deg);
  }
}
}
</style>
