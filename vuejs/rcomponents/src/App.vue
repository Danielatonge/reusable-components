<template>
  <AppButton @click="log">
    <Icon />
    CLICK
  </AppButton>
</template>

<script>
import AppButton from "@/components/AppButton";
import Icon from "@/components/Icon";

export default {
  name: "App",
  components: {
    AppButton,
    Icon
  },
  methods: {
    log() {
      console.log("works");
    }
  }
};
</script>

<style></style>
