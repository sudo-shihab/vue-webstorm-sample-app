<template>
  <div class="tabs is-centered">
    <ul>
      <li
        v-for="(menu, index) in menuList"
        :key="`menu${index}`"
        v-bind:class="[index === 0 ? 'is-active' : '']"
      >
        <a> {{ menu }} </a>
      </li>
    </ul>
  </div>
</template>

<style scoped lang="scss"></style>

<script>
export default {
  name: "app-tabs",
  props: {
    menuList: {
      type: Array,
      default: () => ["shihab"]
    }
  }
};
</script>
