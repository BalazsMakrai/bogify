<template>
  <div>
    <div
      class="w-[calc(100%-240px)] h-[60px] fixed right-0 z-20 bg-[#101010] bg-opacity-80 flex items-center justify-between"
    >
      <div class="items-center ml-6 flex">
        <button
          type="button"
          class="rounded-full bg-black p-[1px] cursor-pointer"
        >
          <ChevronLeft fillColor="#FFFFFF" :size="30" />
        </button>
        <button
          type="button"
          class="rounded-full bg-black p-[1px] cursor-pointer ml-4"
        >
          <ChevronRight fillColor="#FFFFFF" :size="30" />
        </button>
      </div>
      <button
        @click="toggleMenu"
        :class="openMenu ? 'bg-[#282828]' : 'bg-black'"
        class="rounded-full bg-black hover:bg-[#282828] p-0.5 mr-8 mt-0.5 cursor-pointer"
      >
        <div class="flex items-center">
          <img
            class="rounded-full"
            src="https://yt3.ggpht.com/yti/AHyvSCC087C8Qmyp3f5T2tKz1WJOqYjpVZeUJ8U0gkwA4w=s88-c-k-c0x00ffffff-no-rj-mo"
            width="27"
          />
          <div class="text-white text-[14px] ml-1.5 font-semibold">
            Makrai Balázs
          </div>
          <ChevronDown
            v-if="!openMenu"
            @click="toggleMenu"
            fillColor="#FFFFFF"
            :size="25"
          />
          <ChevronUp
            v-else
            @click="toggleMenu"
            fillColor="#FFFFFF"
            :size="25"
          />
        </div></button
      ><span
        v-if="openMenu"
        class="fixed w-[190px] bg-[#282828] shadow-2xl z-50 rounded-sm top-[52px] right-[35px] p-1 cursor-pointer"
      >
        <ul class="text-gray-200 font-semibold text-[14px]">
          <li
            class="px-3 py-2.5 hover:bog-[#3E3D3D] border-b border-b-gray-600"
          >
            Profile
          </li>
          <li class="px-3 py-2.5 hover:bog-[#3E3D3D]">Log out</li>
        </ul></span
      >
    </div>

    <div id="SideNav" class="p-6 h-[100%] w-[240px] fixed z-50 bg-black">
      <RouterLink to="/">
        <img src="/images/icons/spotify-logo.png" width="125" />
      </RouterLink>
      <div class="my-8"></div>
      <RouterLink to="/">
        <MenuItem class="ml-[1px]"  name="Home" iconString="home" pageUrl="/" :iconSize="23"/>
      </RouterLink>
    </div>
  </div>
</template>
<script setup>
import { ref, onMounted } from "vue";
import { RouterLink, RouterView } from "vue-router";
import ChevronUp from "vue-material-design-icons/ChevronUp.vue";
import ChevronDown from "vue-material-design-icons/ChevronDown.vue";
import ChevronRight from "vue-material-design-icons/ChevronRight.vue";
import ChevronLeft from "vue-material-design-icons/Chevronleft.vue";
import MenuItem from "./components/MenuItem.vue";
const openMenu = ref(false);
const toggleMenu = () => {
  openMenu.value = !openMenu.value;
};
</script>
