<template>
  <v-img
    :height="size"
    src="https://camo.githubusercontent.com/7df9af715180067222bc677bdbabfb6edb6c0f29/68747470733a2f2f66696c652e697669657775692e636f6d2f766965772d75692d6c6f676f2d6e65772e737667"
    :width="size"
    class="mx-auto"
    :contain="true"
    max-width="100%"
  />
</template>

<script>
  export default {
    name: 'HomeVuetifyLogo',

    inject: ['theme'],

    computed: {
      size () {
        // return this.$vuetify.breakpoint.smAndUp ? 400 : 250
        return 300
      },
    },
  }
</script>
