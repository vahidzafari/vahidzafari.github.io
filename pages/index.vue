<template>
  <v-container class="pa-8 bg">
    <header class="pa-2">
      <topnav></topnav>
    </header>
    <v-main>
      <v-row class="pa-3">
        <v-col cols="12" sm="6" md="6" lg="4">
          <extra-information></extra-information>
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
import ExtraInformation from '@/components/extra-information.vue'

export default {
  components: {
    topnav,
    Experience,
    ExtraInformation,
  },
}
</script>

<style lang="scss">
.bg {
  background-color: #ffe082 !important;
}
</style>
