<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <b-navbar toggleable="md" type="dark" variant="danger">
      <b-container>
        <b-navbar-brand href="#">NavBar</b-navbar-brand>
        <b-navbar-toggle target="nav_collapse">
        </b-navbar-toggle>
        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item :to="{name: 'Home'}" exact>Home</b-nav-item>
            <b-nav-item :to="{name: 'About'}">About</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-container>
    </b-navbar>
    <router-view/>
  </div>
</template>
<style>
  .router-link-exact-active {
    color: white !important;
  }
</style>