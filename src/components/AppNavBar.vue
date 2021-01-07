<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <a class="navbar-item" href="https://bulma.io">
        <p class="has-text-weight-bold is-size-5">{{ brandName} }</p>
      </a>

      <a
        role="button"
        class="navbar-burger"
        aria-label="menu"
        aria-expanded="false"
        data-target="navbarBasicExample"
      >
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>

    <div id="navbarBasicExample" class="navbar-menu">
      <div class="navbar-start">
        <router-link to="/" class="navbar-item is-active">
          Home Page
        </router-link>

        <router-link to="/about" class="navbar-item">
          About Page
        </router-link>
      </div>

      <div class="navbar-end">
        <div class="navbar-item">
          <div class="buttons">
            <slot name="primary-button"></slot>
            <slot name="sec-button"></slot>
          </div>
        </div>
      </div>
    </div>
  </nav>
</template>
<script>
export default {
  name: "app-header",
  props: {
    brandName: {
      type: String
    }
  }
};
</script>
