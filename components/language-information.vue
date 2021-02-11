<template>
  <section class="Languages">
    <hr />
    <h1>Languages</h1>
    <v-list color="transparent" dense>
      <v-list-item v-for="(item, i) in items" :key="i" dense>
        <v-list-item-avatar class="pa-0 ma-0">
          <v-icon v-text="item.icon"></v-icon>
        </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title v-text="item.title"></v-list-item-title>
        </v-list-item-content>
      </v-list-item>
    </v-list>
  </section>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: 'Persian (Native)',
          icon: 'mdi-web-box',
        },
        {
          title: 'English (Advanced)',
          icon: 'mdi-web-box',
        },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.Languages {
  & > h1 {
    margin: 5px 0;
  }
}
</style>
