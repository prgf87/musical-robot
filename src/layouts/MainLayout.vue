<template>
  <q-layout view="hHh Lpr lFf">
    <q-header>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="mdi-menu"
          aria-label="Menu"
          @click="toggleLeftDrawer"
        ></q-btn>
        <q-toolbar-title> My Todo App </q-toolbar-title>
        <q-btn icon="mdi-logout" flat round dense></q-btn>
      </q-toolbar>
    </q-header>
    <q-drawer
      v-model="leftDrawerOpen"
      show-if-above
      bordered
      class="text-grey-7"
    >
      <q-list>
        <q-toolbar class="bg-primary"></q-toolbar>
        <q-item class="bg-grey-3">
          <q-item-section>Lists</q-item-section>
          <q-item-section side
            ><q-btn icon="mdi-plus" flat round size="sm"></q-btn>
          </q-item-section>
        </q-item>
        <q-item clickable>
          <q-item-section side>
            <q-icon name="mdi-shopping" color="blue-13"></q-icon>
          </q-item-section>
          <q-item-section> Shopping List </q-item-section>
          <q-item-section side> 12 </q-item-section>
        </q-item>
      </q-list>
    </q-drawer>
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script setup lang="ts">
import { ref } from "vue";

const leftDrawerOpen = ref(false);
function toggleLeftDrawer() {
  leftDrawerOpen.value = !leftDrawerOpen.value;
}
</script>
