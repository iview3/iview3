<template>
  <app-menu
    key="learn-menu"
    :items="items"
  >
    <template #activator="{ attrs, on }">
      <app-btn
        v-bind="attrs"
        v-on="on"
      >
        {{ $t('learn') }}

        <app-chevron-down />
      </app-btn>
    </template>
  </app-menu>
</template>

<script>
  export default {
    name: 'LearnMenu',

    computed: {
      items () {
        return [
          { heading: this.$t('documentation') },
          {
            title: this.$t('guide'),
            to: {
              name: 'Documentation',
              params: {
                category: 'introduction',
                page: 'why-vuetify',
              },
              hash: '#guide',
            },
          }
        ]
      },
    },
  }
</script>
