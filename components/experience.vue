<template>
  <section class="experience">
    <hr />
    <h1>Work Experience</h1>
    <v-row>
      <v-col
        v-for="(item, i) in items"
        :key="i"
        cols="12"
        sm="12"
        md="12"
        lg="6"
        class="ma-0 pa-0"
      >
        <v-list color="transparent" two-line dense>
          <v-list-item>
            <template #default>
              <v-list-item-content>
                <v-list-item-title
                  class="subtitle-1"
                  v-text="item.title"
                ></v-list-item-title>

                <v-list-item-subtitle
                  class="text--primary"
                  v-text="item.headline"
                ></v-list-item-subtitle>

                <p
                  class="mt-2 paragraph text--secondary"
                  v-text="item.description"
                ></p>
              </v-list-item-content>
            </template>
          </v-list-item>
        </v-list>
        <v-divider></v-divider>
      </v-col>
    </v-row>
  </section>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          title: 'Full-stack Developer / Agah E-commerce',
          headline: 'Tehran, Iran / Sep 2020- Present',
          description: `Working as a full-stack developer to run kong gateway, debug some 
          issue, help coworkers to write unit test and integration test, 
          luanch bitcoin node along with its APIs for a PSP`,
        },
        {
          title: 'Freelancer / Moshaverline',
          headline: 'Tehran, Iran / Nov 2020 - Dec 2020',
          description: `Working on frontend with Vue.js tools for moshaverline.com
          to run a WebRTC, Vuex, i18n, RBAC, ...`,
        },
        {
          title: 'Frontend Web Developer / Eposnese',
          headline: 'Tehran, Iran / Jan 2019 - Sep 2020',
          description: `Working on an E-commerce website (written in Vue.js), 
            Web Socket dispatcher (written in node.js)`,
        },
        {
          title: 'Web Developer / Shatel',
          headline: 'Tehran, Iran / Feb 2017 - Sep 2018',
          description: `Working on python, Django, and Flask Frameworks`,
        },
        {
          title: 'Assistant It Manager / Hyperstar',
          headline: 'Tehran, Iran / Feb 2016 - Oct 2016',
          description: `Maintaining Cisco switches and routers, computers, printers, 
            web services, and other servers`,
        },
        {
          title: 'Freelancer / Home',
          headline: 'Tehran, Iran / Jul 2015 - Dec 2015',
          description: `Web developer worked as a freelancer at home, 
          and trying to raise my programming skills`,
        },
        {
          title: 'Python Developer / Fanava DP',
          headline: 'Tehran, Iran / Jan 2012 - Apr 2015',
          description:
            'Working on python application and also working on web applications',
        },
      ],
    }
  },
}
</script>

<style lang="scss" scoped>
.experience {
  & > h1 {
    margin: 5px 0;
  }

  .paragraph {
    text-align: justify;
  }
}
</style>
