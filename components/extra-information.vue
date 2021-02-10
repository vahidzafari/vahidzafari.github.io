<template>
  <section class="contact">
    <hr />
    <h1>Contact Me</h1>
    <v-list dense>
      <v-list-item v-for="(item, i) in items" :key="i" :href="item.href" dense>
        <v-list-item-icon>
          <v-icon v-text="item.icon"></v-icon>
        </v-list-item-icon>
        <v-list-item-content>
          <v-list-item-title v-text="item.text"></v-list-item-title>
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
          text: 'zafarivahid@gmail.com',
          icon: 'mdi-gmail',
          href: 'mailto:zafarivahid@gmail.com',
        },
        {
          text: '+98 (912) 814 9776',
          icon: 'mdi-whatsapp',
          href: 'https://wa.me/00989128149776',
        },
        {
          text: 'https://www.linkedin.com/in/vahid-zafari',
          icon: 'mdi-linkedin',
          href: 'https://www.linkedin.com/in/vahid-zafari',
        },
        {
          text: 'https://vahidzafari.github.io',
          icon: 'mdi-web',
          href: 'https://vahidzafari.github.io',
        },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.contact {
  & > h1 {
    margin: 5px 0;
  }
}
</style>
