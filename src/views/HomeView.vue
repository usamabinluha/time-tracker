<template>
  <div class="home">
    <main-page />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import MainPage from "@/components/MainPage.vue";

export default defineComponent({
  name: "HomeView",
  components: {
    MainPage,
  },
});
</script>
