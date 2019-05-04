<template>
  <header>
    <b-navbar 
      toggleable="lg" 
      type="light" 
      variant="light">
      <b-navbar-brand href="/">Git Practice</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"/>

      <b-collapse 
        id="nav-collapse" 
        is-nav>
        <b-navbar-nav>
          <b-nav-item to="list">List</b-nav-item>
        </b-navbar-nav>
      </b-collapse>

    </b-navbar>
  </header>
</template>

<style lang="scss">
@import './node_modules/bootstrap/scss/functions';
@import './node_modules/bootstrap/scss/variables';
@import './node_modules/bootstrap/scss/mixins';

.navbar-light .navbar-nav .nav-link {
  @include hover {
    color: $teal;
  }
  &.nuxt-link-active {
    color: $teal;
  }
}
</style>
