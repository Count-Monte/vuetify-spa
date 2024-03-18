<template>
  <v-app
    theme="myCustomTheme"
    class="bg-grey-darken-4 px-0"
  >
    <v-container
      class="mx-auto pa-0"
      style="max-width: 1200px"
    >
      <v-toolbar class="pl-5">
        <template #prepend>
          <div class="text-h4 font-weight-bold my-5 red text-red-darken-2">
            Landing Page
          </div>
        </template>

        <template #append>
          <div class="hidden-sm-and-down">
            <v-btn
              v-for="item in menu"
              :key="item"
              variant="text"
              class="text-body-1 blue-grey-darken-4"
            >
              {{ item }}
            </v-btn>
          </div>
        </template>
      </v-toolbar>

      <LandingSection />
      <LogoSection />
      <WhatWeDoSection />
      <DiscoverHelp />
      <CustomizeSection />
      <FunFactsSection />
      <WhatPeopleSaySection />
      <OurPortfolioSection />
      <MeetOurTeamSection />
      <AwardWinningSection />
      <AmazingFeaturesSection />
      <PricingSection />
      <FAQSection />
      <ContactUsSection />

      <v-footer class="pa-8">
        <div class="text-body-1">
          2021 <b>Landing Page</b>. Designed by Christopher Saburo
        </div>
      </v-footer>
    </v-container>
  </v-app>
</template>

<script setup>
const menu = [
  "Home",
  "About",
  "Testimonals",
  "Work",
  "Team",
  "Features",
  "Pricing",
];

</script>
