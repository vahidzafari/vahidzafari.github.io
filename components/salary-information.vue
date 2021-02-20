<template>
  <section class="Languages">
    <hr />
    <h1>Salary Expectation</h1>
    <v-list color="transparent" dense>
      <v-list-item v-for="(item, i) in items" :key="i" dense>
        <v-list-item-content>
          <v-list-item-subtitle>{{ item.title }}</v-list-item-subtitle>
          <v-list-item-title>{{ item.value }}</v-list-item-title>
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
          title: 'Expected Salary: ',
          value: '200.000.000 IRR',
        },
        {
          title: 'Payment Period: ',
          value: 'Per month',
        },
        {
          title: 'Mobility Desire: ',
          value: 'Yes, as needed',
        },
        {
          title: 'Notice Period: ',
          value: '4 week',
        },
        {
          title: 'Working hours: ',
          value: '44 hours per week',
        },
        {
          title: 'Employment Type: ',
          value: 'Full-time',
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
