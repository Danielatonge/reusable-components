<template>
  <div>
    <header>
      <slot name="header" />
    </header>
    <main>
      <slot />
    </main>
    <footer>
      <slot name="footer">made with slots</slot>
    </footer>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped></style>
