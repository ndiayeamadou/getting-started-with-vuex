<template>
  <div class="home">
    <img alt="Vue logo" src="../assets/logo.png">
  </div>
  <div>
    <h2>{{ counter }}</h2>
    <div class="buttons">
      <button @click="decrement">-</button>
      <button v-on:click="increment">+</button>
    </div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  data() {
    return {
      counter: 0
    }
  },
  methods: {
    increment() {
      this.counter++
    },
    decrement() {
      this.counter--
    }
  }
}
</script>
