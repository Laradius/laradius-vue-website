<template>
  <div class="container-fluid main-nav text-center">
    <a href="#">
      <img src="./assets/logo.png" alt="logo" height="80" />
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

  <router-view />
</template>

<style>
:root {
  --site-background: #303030;
  --paper-background: #424242;
  --primary: #8c3bc4;
  --primary-text: #fff;
  --primary-hover: rgba(255, 255, 255, 0.9);
  --primary-secondary-text: rgba(255, 255, 255, 0.7);
  --secondary: #73c43b;
  --secondary-text: rgba(0, 0, 0, 0.87);
}

body {
  background-color: var(--site-background) !important;
}

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
