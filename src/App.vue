<template>
  <div id="app">
    <div class="container">
      <ParentComponent />
    </div>
  </div>
</template>

<script>
import ParentComponent from './components/ParentComponent.vue';

export default {
  name: 'App',
  components: {
    ParentComponent,
  },
};
</script>

<style>

body {
  background: linear-gradient(270deg, #aa00ff, #000000, #590031);
  background-size: 600% 600%;
  animation: GradientAnimation 15s ease infinite;
}

@keyframes GradientAnimation {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}

#app {
  font-family: 'Times New Roman', Times, serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #ffffff;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
}

.container {
  width: 600px;
  height: 300px;
  background-color: #3c0058;
  border-radius: 15px;
  box-shadow: 0 0 20px rgba(255, 255, 255, 0.5);
  padding: 20px;
  box-sizing: border-box;
  text-align: center;
  justify-content: center;
}

</style>