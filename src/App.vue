<template lang="pug">
router-view()
</template>

<script lang="ts" setup>
const useLogger = (id: string) => {
  return {
    log(...msg: any[]) {
      console.log(`[${id}]`, ...msg)
    },
  }
}
provide('useLogger', useLogger)
</script>
