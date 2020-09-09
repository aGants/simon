<template>
  <div class="main">
    <div class="game">
      <div class="game-block red"></div>
      <div class="game-block blue"></div>
      <div class="game-block green"></div>
      <div class="game-block yellow"></div>
    </div>
    <div class="setting">
      <button class="btn">Старт</button>
      <p>Раунд: <b>{{ round }}</b></p>
      <label class="label">
        <input type="radio" name='lvl' value='easy' class='radio' v-model='lvl'> Лёгкий
      </label>
      <label class="label">
        <input type="radio" name='lvl' value='medium' class='radio' v-model='lvl'> Средний
      </label>
      <label class="label">
        <input type="radio" name='lvl' value='hard' class='radio' v-model='lvl'> Сложный
      </label>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Game',
  data() {
    return {
      round: 0,
      lvl: 'easy',
    }
  }
}
</script>