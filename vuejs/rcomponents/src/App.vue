<template>
  <AppLayout>
    <template #header> Slots are awesome </template>
    <template #default>
      <AppUserList>
        <!-- <template #loading>
          <AppSpinner> </AppSpinner>
        </template> -->
        <template #secondrow="{ remove, item: user }">
          <AppButton @click="remove(user)">{{ user.name.first }}</AppButton>
        </template>
      </AppUserList>
    </template>
  </AppLayout>
</template>

<script>
// import AppSpinner from "@/components/AppSpinner";
// import Icon from "@/components/Icon";
import AppLayout from "@/components/AppLayout";
import AppButton from "@/components/AppButton";
import AppUserList from "@/components/AppUserList";

export default {
  name: "App",
  components: {
    // AppSpinner,
    // Icon,
    AppButton,
    AppLayout,
    AppUserList,
  },
  methods: {
    log() {
      console.log("works");
    },
  },
};
</script>

<style></style>
