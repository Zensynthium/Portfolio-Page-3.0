<template>
  <div>
  <!-- Change toggleable to md at deployment -->
  <b-navbar class="navbar" toggleable="md" type="dark">
    <b-navbar-brand class="special-text">A. Heggin</b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav>

      <!-- Right aligned nav items -->
      <b-navbar-nav class="ml-auto">
        <b-nav-item class="smooth-select" href="#home">Home</b-nav-item>
        <b-nav-item class="smooth-select" href="#projects">Projects</b-nav-item>
        <b-nav-item class="smooth-select" href="#about">About Me</b-nav-item>
        <b-nav-item class="smooth-select" href="#contact">Contact</b-nav-item>
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

  a:hover {
    transition: all 0.5s ease-out;
  }

  .special-text {
    font-family: "Balista";
    font-size: 17px;
    cursor: default;
  }

  .navbar {
    background-color: black;
    -webkit-box-shadow:0 0 10px rgba(0, 0, 0, 0.5);
	  -moz-box-shadow:0 0 10px rgba(0, 0, 0, 0.5);
	  box-shadow:0 0 10px rgba(0, 0, 0, 0.5);
  }
</style>