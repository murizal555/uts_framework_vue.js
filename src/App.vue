<script setup>
  import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <nav class="navbar navbar-expand-lg bg-light">
      <div class="container-fluid">
        <RouterLink class="navbar-brand green" to="/">Tugas UTS</RouterLink>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarSupportedContent"
          aria-controls="navbarSupportedContent"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav me-auto mb-2 mb-lg-0">
            <li class="nav-item">
              <RouterLink class="nav-link green" aria-current="page" to="/"
                >Galery</RouterLink
              >
            </li>
            <li class="nav-item">
              <RouterLink class="nav-link green" aria-current="page" to="/lives"
                >Lives</RouterLink
              >
            </li>
            <li class="nav-item">
              <RouterLink
                class="nav-link green"
                aria-current="page"
                to="/skills"
                >Skills</RouterLink
              >
            </li>
            <li class="nav-item">
              <RouterLink class="nav-link green" aria-current="page" to="/about"
                >About</RouterLink
              >
            </li>
          </ul>
          <form class="d-flex" role="search">
            <input
              class="form-control me-2"
              type="search"
              placeholder="Search"
              aria-label="Search"
            />
            <button class="btn btn-outline-success" type="submit">
              Search
            </button>
          </form>
        </div>
      </div>
    </nav>
  </header>

  <RouterView />
</template>
