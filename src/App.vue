<template>
  <div id="app">
    <div class="main">
      <div class="color-guide">
        <h5>Color Guide</h5>
        <div class="user user">User</div>
        <div class="user guest">Guest</div>
      </div>
      <canvas v-canvas></canvas>
    </div>
  </div>
</template>

<script>
import canvas from './canvas.directive.js';

export default {
  name: 'app',
  directives: {
    canvas,
  },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
canvas {
  background: navy;
}
.main {
  display: flex;
  justify-content: center;
}

.color-guide {
  margin: 20px 40px;
}

h5 {
  margin-bottom: 10px;
}

.user {
  padding: 7px 15px;
  border-radius: 4px;
  color: white;
  font-size: 13px;
  font-weight: bold;
  background: red;
  margin: 10px 0;
}

.guest {
  background: greenyellow;
  color: black;
}
</style>
