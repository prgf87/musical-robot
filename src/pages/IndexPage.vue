<template>
  <q-page class="row">
    <q-card class="col-xs-9">
      <q-toolbar>
        <q-input
          dense
          class="full-width"
          placeholder="Search"
          :model-value="search"
        >
          <template #append> <q-icon name="mdi-magnify" /> </template>
        </q-input>
      </q-toolbar>
      <TodosList />
    </q-card>
    <div class="col-xs-3">
      <q-toolbar class="bg-primary">
        <TodoButton
          icon="mdi-plus"
          fab
          color="secondary"
          class="fab-btn q-ml-lg"
        />
      </q-toolbar>
    </div>
  </q-page>
</template>

<script setup lang="ts">
import TodoButton from "src/components/TodoButton.vue";
import TodosList from "src/components/TodosList.vue";
import { ref } from "vue";

let search = "";
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
.fab-btn {
  margin-bottom: -50px;
}
</style>
