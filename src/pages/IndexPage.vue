<template>
  <q-page padding>
    <q-select
      label="Please choose one"
      outlined
      :options="options"
      v-model="model"
    ></q-select>
    <!-- borderless is also an option for grid stuff or custom css -->
  </q-page>
</template>

<script setup lang="ts">
import { ref } from "vue";

const model: any = ref(null);
const options: string[] = [
  "Hill",
  "Billy",
  "Bob",
  "Trevor",
  "Jerry",
  "Marvin",
  "Melvin",
];
</script>

<style>
.btn {
  background-color: blue;
  color: white;
}
</style>
