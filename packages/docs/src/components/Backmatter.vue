<template>
  <section
    :id="id"
    class="mt-12"
  >
    <related-pages />

    <app-divider class="mt-7 mb-5" />

    <up-next class="mb-4" />

    <!-- <contribute /> -->
  </section>
</template>

<script>
  // Utilities
  import { sync } from 'vuex-pathify'

  export default {
    name: 'Backmatter',

    data: () => ({ id: 'ready-for-more' }),

    computed: {
      toc: sync('pages/toc'),
      text () {
        return this.$t('ready', { url: this.url })
      },
      url () {
        return '/about/meet-the-team/'
      },
    },
  }
</script>
