<template>
  <div>
    <select v-model="selected">
      <option
        v-for="option in options"
        :key="option.value"
        :value="option.value"
      >
        {{ option.label }}
      </option>
    </select>
    <AppUserList>
      <template #[selected]="{ text }">
        <h4>{{ text }}</h4>
      </template>
    </AppUserList>
  </div>
</template>

<script>
// import AppSpinner from "@/components/AppSpinner";
// import Icon from "@/components/Icon";
// import AppLayout from "@/components/AppLayout";
// import AppButton from "@/components/AppButton";
import AppUserList from "@/components/AppUserList";

export default {
  name: "App",
  components: {
    // AppSpinner,
    // Icon,
    // AppButton,
    // AppLayout,
    AppUserList,
  },
  methods: {
    log() {
      console.log("works");
    },
  },
  data() {
    return {
      selected: "first",
      options: [
        { value: "first", label: "first name" },
        { value: "last", label: "last name" },
        { value: "full", label: "full name" },
        { value: "fullWithTitle", label: "full name with title" },
      ],
    };
  },
};
</script>

<style></style>
