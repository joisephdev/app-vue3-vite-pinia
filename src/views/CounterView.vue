<template>
  <h1>
    Counter View {{ counterStore.counter }}
  </h1>

  <button @click="counterStore.incrementBy(2)">+2</button>
  <button @click="counterStore.incrementBy(4)">+4</button>
  <button @click="increaseBy(6)">+6</button>
  <button @click="increaseBy(8)">+8</button>
  <button @click="increaseBy(10)">+10</button>
</template>

<script lang="ts" setup>
import {useCounterStore} from "../stores/CounterStore";

const counterStore = useCounterStore();

const increaseBy = (value: number) => {
  counterStore.incrementBy(10);
}
</script>
