<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div>
    <div>
      <div class="contact border-bottom py-2 d-flex align-items-center gap-5 justify-content-center">
        <div class="d-flex align-items-center gap-1">
          <i class="material-icons m-0 text-orange fs-6">phone</i>
          <small class="m-0">+254 758 163 164</small>
        </div>
        <div class="d-flex align-items-center gap-1">
          <i class="material-icons m-0 text-orange fs-6">email</i>
          <small class="m-0">packageyangu.logistics@gmail.com</small>
        </div>
      </div>
      <nav class="navbar navbar-expand-lg navbar-light bg-white">
        <div class="container">
          <a class="navbar-brand d-flex align-items-center " href="/">
            <img src="/public/logo1.png" alt="" width="160x" height="80px" style="object-fit: contain;">
            
          </a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNav">
              <ul class="navbar-nav ms-auto">
                  <li><small class=""><router-link class="nav-link" :to="{name: 'home'}">Home</router-link></small></li>
                  <li><small class=""><router-link class="nav-link" :to="{name: 'about'}">About us</router-link></small></li>
                  <li><small class=""><router-link class="nav-link" :to="{name: 'services'}">Services</router-link></small></li>
                  <li><small class=""><router-link class="nav-link" to="/">Contact us</router-link></small></li>
              </ul>
              <div class="m">
                <RouterLink to="/get-quote">
                  <button class="btn btn-sm btn-primary">Send a package</button>
                </RouterLink>   
              </div>
          </div>
        </div>
      </nav>
    </div>
    <div class="pt-1">
      <RouterView></RouterView>
    </div>

            <!-- Footer -->
        <footer class="bg-dark text-light py-5 mt-5">
          <div class="container">
            <div class="row">
              <div class="col-md-4">
                <h5>Contact us</h5>
                <p>Email: packageyangu.logistics@gmail.com</p>
                <p>Phone: +254 758 163 164</p>
                <p>Address: Garden Estate, Garden Court, D18A
                  Kanyagia Drive, Off Marurui Rd</p>
              </div>
              <div class="col-md-4">
                <h5>Quick links</h5>
                <ul class="list-unstyled">
                  <li><router-link class="text-decoration-none text-light" :to="{name: 'about'}">About us</router-link></li>
                  <li><router-link class="text-decoration-none text-light" :to="{name: 'services'}">Services</router-link></li>
                  <li><router-link class="text-decoration-none text-light" to="/">Track package</router-link></li>
                </ul>
              </div>
              <div class="col-md-4">
                <h5>Follow us</h5>
                <div class="fs-4">
                  <i class="bi bi-facebook me-3"></i>
                  <i class="bi bi-twitter me-3"></i>
                  <i class="bi bi-instagram"></i>
                </div>
              </div>
            </div>
            <div class="text-center mt-3">
              <small>&copy; 2025 Courier Services. All rights reserved.</small>
            </div>
          </div>
        </footer>
  </div>

</template>

<style scoped>

</style>
