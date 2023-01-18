<script setup>  
import { RouterLink, RouterView } from "vue-router";
import Navbar from "./components/layouts/navbar.vue"
</script>

<template>
  <Navbar />
  <RouterView />
</template>

<style>
@import "@/assets/css/styles.css";
</style>
