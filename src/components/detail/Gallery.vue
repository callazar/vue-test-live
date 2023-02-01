<script setup>

import { ref } from "vue";

const DefaultImage = ref("gallery-1.png");
const galleries = ref([
  { id: 1, Image: "gallery-2.png" },
  { id: 2, Image: "gallery-3.png" },
  { id: 3, Image: "gallery-4.png" },
  { id: 4, Image: "gallery-5.png" },
]);
</script>

<template>
  <section id="gallery">
    <img
      :src="'/src/assets/img/' + DefaultImage"
      alt=""
      class="w-full mt-6 rounded-2xl"
    />
    <div class="grid grid-cols-4 gap-4 mt-4">
      <template v-for="gallery in galeries" :key="gallery.id">
        <div class="overflow-hidden cursor-pointer rounded-2xl">
        <img :src="'/src/assets/img/' + gallery.image" class="w-full" alt="" />
      </div>
      </template>
      
      <!-- <div class="overflow-hidden cursor-pointer ring-2 ring-indigo-500 rounded-2xl">
        <img src="@/assets/img/gallery-3.png" class="w-full" alt="" />
      </div>
      <div class="overflow-hidden cursor-pointer rounded-2xl">
        <img src="@/assets/img/gallery-4.png" class="w-full" alt="" />
      </div>
      <div class="overflow-hidden cursor-pointer rounded-2xl">
        <img src="@/assets/img/gallery-5.png" class="w-full" alt="" />
      </div> -->
    </div>
  </section>
</template>
