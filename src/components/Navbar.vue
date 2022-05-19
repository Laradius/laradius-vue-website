<template>
  <div class="container-fluid main-nav text-center">
    <a href="#">
      <img src="../assets/logo.png" alt="logo" height="100" />
    </a>

    <nav id="nav" class="navbar navbar-expand-lg navbar-dark">
      <div class="justify-content-center container-fluid">
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>

        <div
          class="justify-content-center text-center collapse navbar-collapse"
          id="navbarNav"
        >
          <ul class="navbar-nav">
            <li class="nav-item">
              <router-link class="nav-link" to="/">Home</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/about">About</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </div>
</template>

<script setup lang="ts"></script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.main-nav {
  background-color: var(--primary);
  color: var(--primary-secondary-text);
}

.nav-link {
  padding-left: 10px !important;
  padding-right: 10px !important;
  display: inline-block !important;
  color: var(--primary-text) !important;
  transition: unset !important;
}

.nav-link:hover {
  color: var(--primary-hover) !important;
}

.router-link-exact-active {
  border-bottom: 2px solid var(--secondary);
}
</style>
