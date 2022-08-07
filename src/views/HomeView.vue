<template>
  <h1>
    Home View: {{counterStore.counter}}
  </h1>
  <h3>Número de cambios: {{counterStore.numberOfChanges}}</h3>
</template>

<script lang="ts" setup>
import {useCounterStore} from "../stores/CounterStore";

const counterStore = useCounterStore();
</script>
