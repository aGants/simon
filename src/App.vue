<template>
  <div id="app">
    <Game/>
  </div>
</template>

<script>
import Game from './components/Game.vue'

export default {
  name: 'App',
  components: {
    Game
  }
}
</script>

<style lang="scss">

* {
  margin: 0;
  padding: 0;
}

body {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: Avenir, Helvetica, Arial, sans-serif
}

.game {
  width: 310px;
  height: 320px;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;

  &-block {
    width: 150px;
    height: 150px;
    cursor: pointer;
  }
}

.btn {
  width: 310px;
  height: 30px;
  margin: 20px auto 25px;
  text-align: center;
  cursor: pointer;
  background: #E7ECFF;
  outline: none;
  border: none;
  &:hover {
    border: 2px solid #C6D8FF;
  }
  &:active {
    background: #C6D8FF;
  }
}

.radio {
  margin: 25px 8px;
  cursor: pointer;
}

.label {
  cursor: pointer;
}

.red { background: #FED6BC; &:hover { background: #ffae81; } }
.blue { background: #DEF7FE; &:hover { background: #b8e4f0; } }
.green { background: #C3FBD8; &:hover { background: #a5ecc2; } }
.yellow { background: #FFFADD; &:hover { background: #f6e9b0; } }

</style>
