<template>
  <div>
  <!-- Change toggleable to md at deployment -->
  <b-navbar toggleable="lg" type="dark" variant="dark">
    <b-navbar-brand class="special-text">A. Heggin</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-item class="smooth-select" href="#">Home</b-nav-item>
        <b-nav-item class="smooth-select" href="#">About Me</b-nav-item>
        <b-nav-item class="smooth-select" href="#">Projects</b-nav-item>
        <b-nav-item class="smooth-select" href="#">Contact</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</div>
</template>

<style>
  @font-face {
    font-family: "Balista";
    src: url("../fonts/Balista-2OWro.ttf") format("truetype");
  }

  .special-text {
    font-family: "Balista";
    font-size: 17px;
    cursor: default;
  }

  a:hover {
    transition: all 0.6s ease-out;
  }
</style>