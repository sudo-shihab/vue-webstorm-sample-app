<template>
  <div class="about">
    <app-nav-bar-wrapper />
    <app-tabs :menu-list="['sports', 'news']" />
    <hero-page-header
      title="About Us Page"
      sub-title="Description about about page bla"
    />

    <p>shaikh fdklvnl fjvklfdklv j jdkl fv</p>
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
