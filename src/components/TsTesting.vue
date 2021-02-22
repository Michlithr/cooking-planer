<template>
  <div>
    <button v-on:click="decrement">-</button>
    {{ count }}
    <button v-on:click="increment">+</button>
  </div>
</template>

<script lang="ts">
import { Vue } from "vue-class-component";

export default class Counter extends Vue {
  private count = 0;

  increment() {
    this.count++;
  }

  decrement() {
    this.count--;
  }
}
</script>

<style scoped></style>
