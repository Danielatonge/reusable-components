<template>
  <AppLayout>
    <template #header> Slots are awesome </template>
    <template #default>
      <AppUserList :secondrow="(name) => name.email">
        <template #loading>
          <AppSpinner> </AppSpinner>
        </template>
      </AppUserList>
    </template>
  </AppLayout>
</template>

<script>
import AppSpinner from "@/components/AppSpinner";
// import Icon from "@/components/Icon";
import AppLayout from "@/components/AppLayout";
import AppUserList from "@/components/AppUserList";

export default {
  name: "App",
  components: {
    AppSpinner,
    // Icon,
    AppLayout,
    AppUserList
  },
  methods: {
    log() {
      console.log("works");
    }
  }
};
</script>

<style></style>
