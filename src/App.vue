<script setup>
import { RouterLink, RouterView } from "vue-router";
import HelloWorld from "@/components/HelloWorld.vue";
</script>

<template>
  <nav class="bg-white border-gray-200 px-2 sm:px-4 py-2.5 rounded dark:bg-gray-800">
    <div class="container flex flex-wrap items-center justify-between mx-auto my-2">
      <a href="/" class="flex items-center">
        <img src="@/assets/img/logo.svg" class="h-8 ml-3 sm:ml-0 sm:h-8" alt="zullkit logo" />
      </a>
      <div class="md:order-2">
        <a href="login.html"
          class="px-8 py-3 mt-2 mr-2 text-base font-medium text-black bg-gray-200 border border-transparent rounded-full hover:bg-gray-300 md:py-2 md:text-sm md:px-8 hover:shadow">
          Sign In
        </a>
        <a href="register.html"
          class="px-8 py-3 text-base font-medium text-white border border-transparent rounded-full bg-navy hover:bg-navy md:py-2 md:text-sm md:px-8 hover:shadow">
          Sign Up
        </a>
      </div>
      <div class="items-center justify-between hidden w-full md:flex md:w-auto md:order-1" id="mobile-menu-2">
        <ul class="flex flex-col mt-4 md:flex-row md:space-x-8 md:mt-0 md:text-sm md:font-regular">
          <li>
            <RouterLink to="/"
              class="block py-2 pl-3 pr-4 text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-indigo-600 md:p-0 dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700"
              aria-current="page">Home</RouterLink>
          </li>
          <li>
            <RouterLink to="/categories"
              class="block py-2 pl-3 pr-4 text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-indigo-600 md:p-0 dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">Categories</RouterLink>
          </li>
          <li>
            <RouterLink to="/pricing"
              class="block py-2 pl-3 pr-4 text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-indigo-600 md:p-0 dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">Pricing</RouterLink>
          </li>
          <li>
            <a href="#"
              class="block py-2 pl-3 pr-4 text-gray-700 border-b border-gray-100 hover:bg-gray-50 md:hover:bg-transparent md:border-0 md:hover:text-indigo-600 md:p-0 dark:text-gray-400 md:dark:hover:text-white dark:hover:bg-gray-700 dark:hover:text-white md:dark:hover:bg-transparent dark:border-gray-700">Study
              Case</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

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
