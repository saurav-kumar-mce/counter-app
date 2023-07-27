<template>
  <div class="counter-app">
    <h1>Counter App</h1>
    <div class="counter">
      <button @click="decrement">-</button>
      <span>{{ count }}</span>
      <button @click="increment">+</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      count: 0
    };
  },
  methods: {
    increment() {
      this.count++;
    },
    decrement() {
        this.count--;
      }
    }
  };
</script>

<style>
.counter-app {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100vh;
}

.counter {
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 24px;
}

button {
  margin: 0 10px;
  padding: 10px 20px;
  font-size: 18px;
  cursor: pointer;
}
</style>
