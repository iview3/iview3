<template>
  <app-btn
    :to="{
      name: 'Documentation',
      params: {
        category: 'getting-started',
        page: 'installation'
      }
    }"
    path="guide"
  />
</template>

<script>
  export default { name: 'StartLink' }
</script>
