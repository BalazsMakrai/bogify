<template>
  <div class="p-8">
    <button
      type="button"
      class="text-white text-2xl gont-semibold hover:underline cursor-pointer"
    >
      Recommended genres
    </button>
    <div class="py-1.5"></div>
    <div
      class="grid xl:grid-cols-5 lg:grid-cols-4 md:grid-cols-3 sm:grid-cols-2 gap-6"
    >
      <CategorySelect
        v-for="genre in genres"
        :key="genre.id"
        :category="genre.category"
        :image="`https://picsum.photos/id/${genre.id}/300/300`"
      />
    </div>
  </div>
</template>

<script setup>
import CategorySelect from "../components/CategorySelect.vue";
import musicGenres from "../data/categories.json";
const genres=musicGenres.sort((a,b)=>a.id-b.id);
</script>
