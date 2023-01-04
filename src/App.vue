<script setup>  
import { RouterLink, RouterView } from "vue-router";
import Navbar from "./components/layouts/navbar.vue"
</script>

<template>
  <Navbar />
  <RouterView />

  <!-- panding start -->
  <!-- <header>
      <nav>
        <RouterLink to="/">Home</RouterLink>
      </nav>
  </header> -->
  <!-- panding end -->
</template>

<style>
@import "@/assets/css/styles.css";
</style>
