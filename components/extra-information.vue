<template>
  <section class="contact">
    <hr />
    <h1>Contact Me</h1>
    <v-list color="transparent" dense>
      <v-list-item v-for="(item, i) in items" :key="i" :href="item.href" dense>
        <v-list-item-avatar>
          <v-icon v-text="item.icon"></v-icon>
        </v-list-item-avatar>
        <v-list-item-content>
          <v-list-item-title v-html="item.title"></v-list-item-title>
          <v-list-item-subtitle v-html="item.subtitle"></v-list-item-subtitle>
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
          title: 'E-mail',
          subtitle: 'zafarivahid@gmail.com',
          icon: 'mdi-gmail',
          href: 'mailto:zafarivahid@gmail.com',
        },
        {
          title: 'Whats App',
          subtitle: '+98 (912) 814 9776',
          icon: 'mdi-whatsapp',
          href: 'https://wa.me/00989128149776',
        },
        {
          title: 'Linkedin',
          subtitle: 'https://www.linkedin.com/in/vahid-zafari',
          icon: 'mdi-linkedin',
          href: 'https://www.linkedin.com/in/vahid-zafari',
        },
        {
          title: 'Portfolio',
          subtitle: 'https://vahidzafari.github.io',
          icon: 'mdi-web',
          href: 'https://vahidzafari.github.io',
        },
        {
          title: 'Github',
          subtitle: 'https://github.com/vahidzafari',
          icon: 'mdi-web',
          href: 'https://github.com/vahidzafari',
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
