<template>
  <div class="about">
    <app-nav-bar-wrapper />

    <hero-page-header
      title="About Us Page"
      sub-title="Description about about page bla"
    />
        <app-tabs :menu-list="['sports', 'news']" />
  </div>
</template>

<script>
import AppNavBarWrapper from "@/components/AppNavBarWrapperr";
import HeroPageHeader from "@/components/HeroPageHeader";
import AppTabs from "@/components/AppTabs";

export default {
  name: "About",
  components: { AppNavBarWrapper, HeroPageHeader, AppTabs }
};
</script>

<style></style>
