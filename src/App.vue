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
  --primary: #8c3bc4;
  --primary-text: #fff;
  --secondary: #73c43b;
  --secondary-text: rgba(0, 0, 0, 0.87);
}

.main-nav {
  background-color: var(--primary);
  color: var(--primary-text);
}
</style>
