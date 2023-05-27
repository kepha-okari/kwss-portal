<template>
  <div>
    <b-navbar toggleable="lg" sticky  variant="light" type="light">
      <b-navbar-brand href="/">
        <img
          src="../assets/add.png"
          alt=""
          class="nav-img"
      />KWSS</b-navbar-brand>

      <b-navbar-toggle target="nav-collapse" style="background-color: #fff"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
          <b-navbar-nav class="menu">
            <b-nav-item href="/"><span>Home</span></b-nav-item>
            <b-nav-item href="/readings"><span>Add Readings</span></b-nav-item>
            <b-nav-item href="/billing"><span>Send Bills</span></b-nav-item>
          </b-navbar-nav>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>
<style>
/* home route and active route will show in bold as it matches / and /about */
a.nuxt-link-active {
  font-weight: bold;
  color: cyan;
}
/* exact link will show the primary color for only the exact matching link */
a.nuxt-link-exact-active {
  color: #00c58e;
}
.nuxt-link-prefetched {
  color: orangeRed;
}
span {
  color: #2486d6;
}
.nav-img {
  height: 2em;
  width: 2em;
}
</style>
