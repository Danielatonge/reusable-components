<template>
  <button v-on="$listeners">
    <slot></slot>
  </button>
</template>

<script>
export default {
  components: {}
};
</script>

<style scoped></style>
