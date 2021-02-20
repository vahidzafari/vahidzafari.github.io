<template>
  <v-container class="pa-8 bg">
    <header class="pa-2">
      <topnav></topnav>
    </header>
    <v-main>
      <v-row class="pa-3">
        <v-col cols="12" sm="6" md="6" lg="4">
          <contact-information></contact-information>
          <language-information></language-information>
          <salary-information></salary-information>
        </v-col>
        <v-col cols="12" sm="6" md="6" lg="8">
          <experience></experience>
        </v-col>
      </v-row>
    </v-main>
  </v-container>
</template>

<script>
import topnav from '@/components/topnav'
import Experience from '@/components/experience.vue'
import ContactInformation from '@/components/contact-information.vue'
import LanguageInformation from '~/components/language-information.vue'
import SalaryInformation from '~/components/salary-information.vue'

export default {
  components: {
    topnav,
    Experience,
    ContactInformation,
    LanguageInformation,
    SalaryInformation,
  },
}
</script>

<style lang="scss">
.bg {
  border: 2px solid black;
  background-color: #ffe082 !important;
}

.container {
  max-width: 1280px !important;
}
</style>
