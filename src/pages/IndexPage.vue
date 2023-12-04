<template>
  <q-page class="row">
    <q-card class="col-xs-9">
      <q-toolbar>
        <q-input
          class="full-width"
          borderless
          placeholder="Search"
          :model-value="search"
        >
          <template #append> <q-icon name="mdi-magnify" /> </template>
        </q-input>
      </q-toolbar>
      <q-list>
        <q-item>
          <q-item-section side>
            <q-checkbox :model-value="true" />
          </q-item-section>
          <q-item-section> Go Shopping </q-item-section>
          <q-item-section side>
            <q-btn icon="mdi-delete" flat round size="md" color="red"> </q-btn>
          </q-item-section>
        </q-item>
      </q-list>
    </q-card>
  </q-page>
</template>

<script setup lang="ts">
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
</style>
