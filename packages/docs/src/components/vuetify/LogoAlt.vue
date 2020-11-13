<template>
  <router-link
    class="d-inline-block"
    v-bind="$attrs"
    v-on="$listeners"
  >
    <v-img
      src="https://file.iviewui.com/dist/7dcf5af41fac2e4728549fa7e73d61c5.svg"
      :alt="$t('logo')"
      class="shrink"
      max-width="34"
      min-width="34"
      transition="scale-transition"
    />
  </router-link>
</template>

<script>
  export default {
    name: 'VuetifyLogoAlt',

    inject: ['theme'],
  }
</script>
