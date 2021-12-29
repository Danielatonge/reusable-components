<template>
  <AppLayout>
    <template #header> Slots are awesome </template>
    <template #default>
      <AppButton @click="log">
        <Icon />
        CLICK
      </AppButton>
    </template>
  </AppLayout>
</template>

<script>
import AppButton from "@/components/AppButton";
import Icon from "@/components/Icon";
import AppLayout from "@/components/AppLayout";

export default {
  name: "App",
  components: {
    AppButton,
    Icon,
    AppLayout
  },
  methods: {
    log() {
      console.log("works");
    }
  }
};
</script>

<style></style>
