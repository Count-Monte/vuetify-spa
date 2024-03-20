<template>
  <v-sheet
    color="primary"
    height="450px"
    class="text-center px-15 pt-15"
  >
    <div class="text-h3 font-weight-bold mb-5">
      Fun Facts About Our Agency
    </div>
    <v-row class="mx-15">
      <v-col
        v-for="item in agency"
        :key="item.title"
        class="mt-10 d-flex flex-column align-center"
      >
        <v-img
          :src="item.icon"
          width="60"
        />
        <div class="text-h4 font-weight-bold mt-3">
          {{ item.title }}
        </div>
        <div class="text-body-1 mt-2">
          {{ item.description }}
        </div>
      </v-col>
    </v-row>
  </v-sheet>
</template>

<script setup>
const agency = [
  {
    icon: './assets/agency/completed.png',
    title: '1050+',
    description: 'Projects Completed'
  },
  {
    icon: './assets/agency/heart.png',
    title: '217k',
    description: 'Happy Clients'
  },
  {
    icon: './assets/agency/awards.png',
    title: '1210',
    description: 'Design Awards'
  },
  {
    icon: './assets/agency/anchor.png',
    title: '2137',
    description: 'Line Of Codes'
  }
]
</script>
