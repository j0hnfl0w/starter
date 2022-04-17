<style lang="scss" scoped></style>

<template lang="pug">
.row.full-width.bg-red
  h1 PageIndex
  q-btn() Pick me
  q-btn() Hello
</template>

<script setup>
const logger = inject('useLogger')('PageIndex')

onMounted(() => {
  logger.log(':onMounted')
})
</script>
