<template>
  <q-page padding>
    <!-- <q-btn color="blue-10">Click Me</q-btn> -->
    <!-- <q-card style="width: 350px">
      <q-card-section class="bg-blue text-white"> My Card </q-card-section>
      <q-card-section>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequatur
        magni est itaque veniam nihil dignissimos, distinctio deleniti corporis
        veritatis provident, nostrum esse, rerum in ipsam rem numquam ea sint
        quas.
      </q-card-section>
    </q-card> -->
    <q-select
      filled
      :options="['Hill', 'Billy', 'Bob', 'Trevor', 'Jerry', 'Marvin', 'Melvin']"
      v-model="selected"
    ></q-select>
    <!-- <example-component
      title="Example component"
      active
      :todos="todos"
      :meta="meta"
    ></example-component> -->
  </q-page>
</template>

<script setup lang="ts">
import { Todo, Meta } from "components/models";
import { ref } from "vue";

const todos = ref<Todo[]>([
  {
    id: 1,
    content: "ct1",
  },
  {
    id: 2,
    content: "ct2",
  },
  {
    id: 3,
    content: "ct3",
  },
  {
    id: 4,
    content: "ct4",
  },
  {
    id: 5,
    content: "ct5",
  },
]);
const meta = ref<Meta>({
  totalCount: 1200,
});

let selected: string | null = null;
</script>

<style>
.btn {
  background-color: blue;
  color: white;
}
</style>
