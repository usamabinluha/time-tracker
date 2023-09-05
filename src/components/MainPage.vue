<template>
  <div>
    <h1>This is the home page</h1>
    <form @submit.prevent="login">
      <div>
        <label for="username">Username:</label>
        <input type="text" id="username" v-model="username" />
      </div>
      <div>
        <label for="password">Password:</label>
        <input type="password" id="password" v-model="password" />
      </div>
      <div>
        <button type="submit">Login</button>
      </div>
    </form>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "MainPage",
  data() {
    return {
      username: "",
      password: "",
    };
  },
  methods: {
    login() {
      // Handle login logic here using this.username and this.password
      console.log("Username:", this.username);
      console.log("Password:", this.password);
      // Example: Send a login request to the server
    },
  },
});
</script>

<style scoped lang="scss"></style>
