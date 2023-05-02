<template>
  <div>
    <VApp>
      <TopNavigation></TopNavigation>
      <VMain>
        <slot />
      </VMain>
    </VApp>
  </div>
</template>

<script>

export default {
  name: "dashboard",
};
</script>

<style scoped>

</style>