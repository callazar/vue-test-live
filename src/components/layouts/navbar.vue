<script setup>
import logo from "./logo.vue"
import navlink from "./navigationlink.vue"
import userinfo from "./userinfo.vue"
</script>

<template>
    <nav class="bg-white border-gray-200 px-2 sm:px-4 py-2.5 rounded dark:bg-gray-800">
        <div class="container flex flex-wrap items-center justify-between mx-auto my-2">

            <logo />

            <userinfo />

            <navlink />
            
        </div>
    </nav>
</template>