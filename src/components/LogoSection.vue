<template>
  <v-sheet class="py-15 ga-5 d-flex justify-center">
    <div
      v-for="item in banners"
      :key="item.icon"
    >
      <v-img
        :src="item.icon"
        :width="item.width"
        :height="item.height"
      />
    </div>
  </v-sheet>
</template>

<script setup>
const banners = [
  {
    icon: "./assets/banner/csswinner.png",
    width: 150,
    height: 60
  }, {
    icon: "./assets/banner/cssawards.png",
    width: 66,
    height: 61
  }, {
    icon: "./assets/banner/fwa.png",
    width: 133,
    height: 50
  }, {
    icon: "./assets/banner/cssdesignawards.png",
    width: 239,
    height: 53
  }
];
</script>
