<template>
    <q-layout view="hHh lpR fFf">
      <q-header elevated>
        <q-toolbar>
          <q-toolbar-title>
            WEATHER
          </q-toolbar-title>
          <q-space></q-space>
          <q-btn flat round dense>
            t. sela susanti
            <q-icon name="arrow_drop_down" />
            <q-menu>
              <q-list style="min-width: 100px">
                <q-item clickable v-ripple to="/task1">
                  <q-item-section>Tugas 1</q-item-section>
                </q-item>
                <q-item clickable v-ripple to="/task2">
                  <q-item-section>Tugas 2</q-item-section>
                </q-item>
                <q-item clickable v-ripple to="/task3">
                  <q-item-section>Tugas 3</q-item-section>
                </q-item>
                <q-item clickable v-ripple to="/task4">
                  <q-item-section>Tugas 4</q-item-section>
                </q-item>
                <q-item clickable v-ripple to="/task5">
                  <q-item-section>Tugas 5</q-item-section>
                </q-item>
                <q-item clickable v-ripple to="/task6">
                  <q-item-section>Tugas 6</q-item-section>
                </q-item>
                <q-item clickable v-ripple to="/task7">
                  <q-item-section>Tugas 7</q-item-section>
                </q-item>
              </q-list>
            </q-menu>
          </q-btn>
        </q-toolbar>
      </q-header>
  
      <q-page-container>
        <router-view></router-view>
      </q-page-container>
    </q-layout>
  </template>
  
  <script>
  import { ref } from 'vue';
  
  export default {
    name: 'MainLayout',
    setup() {
      const leftDrawerOpen = ref(false);
  
      function toggleLeftDrawer() {
        leftDrawerOpen.value = !leftDrawerOpen.value;
      }
  
      return {
        leftDrawerOpen,
        toggleLeftDrawer,
      };
    },
  };
  </script>
  