<template>
  <div id="app">
    <News :apiKey="apiKey" />
  </div>
</template>

<script>
import News  from "./components/News";
export default {
  name: 'app',
  data: () => {
    return {
      apiKey: '82b816f2ea7847a1a2a8a3dd06fb9003'
    }
  },
  components: {
    News
  }
}
</script>

<style lang="scss">
 @import url('https://use.fontawesome.com/releases/v5.7.2/css/all.css');
 body {
    margin: 0;
    padding: 0;
    width: 100%;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background: linear-gradient(to bottom, #80A248, #198B4D);
  }
  #app {
    font-family: Arial, Helvetica, sans-serif;
    font-size: 1rem;
    color: #333;
    width: 100%;
    max-width: 480px;
    height: 95%;
    max-height: 1000px;
    background-color: #fff;
    overflow-y: scroll;
    overflow-x: hidden;
    
  }
  ::-webkit-scrollbar {
    display: none;
  }
</style>
