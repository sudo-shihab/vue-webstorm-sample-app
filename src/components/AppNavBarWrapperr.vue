<template>
  <AppNavBar brand-name="Vue Webstorm Workflow">
    <template slot="primary-button">
      <a href="" class="button is-primary has-text-weight-bold">Sign up</a>
    </template>
    <template slot="sec-button">
      <a href="" class="button is-light has-text-weight-bold">Login</a>
    </template>
  </AppNavBar>
</template>
<script>
import AppNavBar from "@/components/AppNavBar";

export default {
  name: "AppNavBarWrapper",
  components: { AppNavBar },
  mounted() {
    console.log("hello from mounted fun of AppHeaderWrp component");
  }
};
</script>
