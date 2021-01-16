<template>
  <section :class="['hero', backgroundClass]">
    <div class="hero-body">
      <div class="container">
        <h1 class="title">
          {{ title }}
        </h1>
        <h2 class="subtitle">
          {{ subTitle }}
        </h2>
        <p>
          <button
            class="button is-light"
            @click="colorChange('has-background-primary')"
          >
            Change Color
          </button>
        </p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "HeroPageHeader",
  data() {
    return {
      bgIsToggled: false
    };
  },
  props: {
    subTitle: {
      type: String,
      default: "Sub Title of Page"
    },
    title: {
      type: String,
      default: "Page Header"
    },
    backgroundClass: {
      type: String,
      default: "has-background-warning"
    }
  },
  methods: {
    colorChange(bgCssClass) {
      this.backgroundClass = bgCssClass;
    }
  }
};
</script>

<style scoped></style>
