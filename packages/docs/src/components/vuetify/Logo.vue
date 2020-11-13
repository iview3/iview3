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
      max-width="148"
      width="148"
    />
  </router-link>
</template>

<script>
  export default {
    name: 'VuetifyLogo',

    inject: ['theme'],
  }
</script>
