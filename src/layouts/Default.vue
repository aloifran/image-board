<template>
  <v-app>
    <v-app-bar density="prominent" class="bg-grey-darken-4">
      <v-btn
        variant="outlined"
        prepend-icon="fas fa-plus"
        class="my-10 mx-5"
        @click="store.showDialogForm = !store.showDialogForm"
        >Add an image</v-btn
      >
    </v-app-bar>
    <v-main>
      <router-view />
    </v-main>
    <v-footer class="bg-grey-darken-4 text-grey">Francisco Aloi 2023 </v-footer>
  </v-app>
</template>

<script setup lang="ts">
import { useAppStore } from "@/store/app";

const store = useAppStore();
</script>
