<script setup>
const linkUrl= "https://www.google.com"
const  imageUrl= "https://picsum.photos/seed/picsum/200/300"
</script>

<template>
  <nav
    class="navbar shadow-sm sticky-top navbar-expand-lg navbar-light bg-white py-3"
  >
    <div class="container px-5">
      <a class="navbar-brand" href="{{ url('/') }}"
        ><span class="fw-bolder text-primary">MR-X</span></a
      >
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
        <ul class="navbar-nav ms-auto mb-2 mb-lg-0 small fw-bolder">
          <li class="nav-item">
            <a class="nav-link" href="{{ url('/') }}">Home</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="{{ url('/resume') }}">Resume</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="{{ url('/projects') }}">Projects</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="{{ url('/contact') }}">Contact</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
  <header class="py-5">
    <div class="container px-5 pb-5">
      <div class="row gx-5 align-items-center">
        <div class="col-xxl-5">
          <!-- Header text content-->
          <div class="text-center text-xxl-start">
            <div class="badge bg-gradient-primary-to-secondary text-white mb-4">
              <div id="keyLine" class="text-uppercase">
                Design &middot; Development &middot; Marketing
              </div>
            </div>
            <div id="title" class="fs-3 fw-light text-muted">
              I can help your business to
            </div>
            <h1
              id="short_title"
              class="display-3 fw-bolder mb-5 text-gradient d-inline"
            >
              Get online and grow fast
            </h1>
            <div
              class="d-grid gap-3 d-sm-flex justify-content-sm-center justify-content-xxl-start mb-3"
            >
              <a
                class="btn btn-primary btn-lg px-5 py-3 me-sm-3 fs-6 fw-bolder"
                href="{{ url('/resume') }}"
                >Resume</a
              >
              <a
                class="btn btn-outline-dark btn-lg px-5 py-3 fs-6 fw-bolder"
                href="{{ url('/projects') }}"
                >Projects</a
              >
            </div>
          </div>
        </div>
        <div class="col-xxl-7">
          <div class="d-flex justify-content-center mt-5 mt-xxl-0">
            <div class="profile">
              <img id="profileImg" class="profile-img" src="" alt="..." />
            </div>
          </div>
        </div>
      </div>
    </div>
  </header>
   <div>
    <img :src="imageUrl" alt="My Image" />
      <div>
    <a :href="linkUrl">Click me</a>
  </div>
  </div>
</template>

<style scoped>
@import 'bootstrap/dist/css/bootstrap.min.css';
</style>
