<template>
  <div class="p-8">
    <button
      type="button"
      class="text-white text-2xl gont-semibold hover:underline cursor-pointer"
    >
      Podcast to make you smarter
    </button>
    <div class="py-1.5"></div>
    <div class="flex item-center">
      <HomeCard
        image="https://picsum.photos/id/30/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
      <HomeCard
        image="https://picsum.photos/id/45/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
      <HomeCard
        class="md:block hidden"
        image="https://picsum.photos/id/32/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
      <HomeCard
        class="lg:block hidden"
        image="https://picsum.photos/id/58/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
      <HomeCard
        class="xl:block hidden"
        image="https://picsum.photos/id/57/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
    </div>
  </div>

  <div class="p-8">
    <button
      type="button"
      class="text-white text-2xl gont-semibold hover:underline cursor-pointer"
    >
      Recommended radio
    </button>
    <div class="py-1.5"></div>
    <div class="flex item-center">
      <HomeCard
        image="https://picsum.photos/id/47/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
      <HomeCard
        image="https://picsum.photos/id/72/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
      <HomeCard
        class="md:block hidden"
        image="https://picsum.photos/id/24/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
      <HomeCard
        class="lg:block hidden"
        image="https://picsum.photos/id/11/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
      <HomeCard
        class="xl:block hidden"
        image="https://picsum.photos/id/10/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
    </div>
  </div>

  <div class="p-8">
    <button
      type="button"
      class="text-white text-2xl gont-semibold hover:underline cursor-pointer"
    >
      Recommended songs
    </button>
    <div class="py-1.5"></div>
    <div class="flex item-center">
      <HomeCard
        image="https://picsum.photos/id/78/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
      <HomeCard
        image="https://picsum.photos/id/79/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
      <HomeCard
        class="md:block hidden"
        image="https://picsum.photos/id/88/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
      <HomeCard
        class="lg:block hidden"
        image="https://picsum.photos/id/89/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
      <HomeCard
        class="xl:block hidden"
        image="https://picsum.photos/id/92/300/300"
        title="Title is here"
        subTitle="Subtitle is here"
      />
    </div>
  </div>
</template>

<script setup>
import HomeCard from "../components/HomeCard.vue";
</script>
