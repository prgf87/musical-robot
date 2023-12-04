<template>
  <q-page class="row">
    <div class="bg-blue col-3"></div>
    <div class="bg-orange col-3"></div>
    <div class="bg-red col-6"></div>
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
