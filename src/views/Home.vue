<template>
  <div class="home">
    <!-- Header Section -->
    <section class="header">
      <app-nav-bar-wrapper />
       </section>

    <!-- Main PAge Header -->
    <section class="main-page-header">
      <hero-page-header
        sub-title="Find home page related data here"
        title="Home Page"
      />
    </section>

    <!-- App Tabs -->
    <section>
      <app-tabs :menu-list="['Top Stories', 'Politics', 'Movie']" />
    </section>

    <!-- Main Section -->
    <section class="main-area"></section>
  </div>
</template>

<script>
import AppTabs from "@/components/AppTabs";
import AppNavBarWrapper from "@/components/AppNavBarWrapperr";
import HeroPageHeader from "@/components/HeroPageHeader";

export default {
  name: "Home",
  components: { AppNavBarWrapper, HeroPageHeader, AppTabs },
  created() {
    console.log("hello from home.vue");
  }
};
</script>

<style lang="scss" scoped>
.wrp {
  padding: 15px;
}
</style>
