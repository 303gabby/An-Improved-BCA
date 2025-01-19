<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div class="page-wrapper">
    <header>
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/academics">Academics</RouterLink>
        <RouterLink to="/admissions">Admission</RouterLink>
        <RouterLink to="/students">Students</RouterLink>
        <RouterLink to="/parents">Parents</RouterLink>
        <RouterLink to="/contact">Contact Us</RouterLink>
      </nav>
    </header>
    
    <main class="main-content">
      <RouterView />
    </main>

    <footer class="footer">
    <div class="footer-content">
      <!-- Left Column with Logos -->
      <div class="logo-column">
        <img src="@/assets/Brooklyn_College_Seal.svg" alt="Seal of Brooklyn College" class="college-seal">
        <img src="@/assets/NYC DOE.png" alt="NYC Department of Education Logo" class="doe-logo">
      </div>

      <!-- Middle Column -->
      <div class="info-column">
        <h2>Main Site (Grades 9-10)</h2>
        <p>350 Coney Island Ave, Brooklyn NY 11218</p>
        <p>Email: bcaconnection@brooklyncollegeacademy.com</p>
        <p>Phone: (718) 853 6184</p>
        <p>Fax: (718) 853 6356</p>
      </div>

      <!-- Right Column -->
      <div class="info-column">
        <h2>Campus Site (Grades 11-12)</h2>
        <p>2900 Bedford Ave, Brooklyn NY 11230</p>
        <p>Email: bcaconnection@brooklyncollegeacademy.com</p>
        <p>Phone: (718) 951 5941</p>
        <p>Fax: (718) 951 4441</p>
      </div>

      <!-- Social Icons -->
      <div class="social-icons">
        <a href="mailto:bcaconnection@brooklyncollegeacademy.com">
          <img src="@/assets/envelope.svg" alt="Email" class="social-icon">
        </a>
        <a href="https://www.instagram.com/bca.world/">
          <img src="@/assets/instagram-logo.svg" alt="Instagram" class="social-icon">
        </a>
      </div>
    </div>
  </footer>
  </div>
</template>

<style scoped>
.page-wrapper {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

.main-content {
  flex: 1;
  padding: 1rem;
}

header {
  position: sticky;
  top: 0;
  z-index: 1000;
  background-color: #FFFF;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
  padding: 1rem 0;
}

nav a {
  display: inline-block;
  padding: 0.5rem 1rem;
  text-decoration: none;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

nav a.router-link-exact-active {
  color: #74218A;
}

nav a.router-link-exact-active:hover {
  background-color: #74218A;
  color: #FFFF;
}

.footer {
  background-color: #74218A;
  color: white;
  padding: 2rem 0;
  width: 100%;
  margin-top: auto;
}

.footer-content {
  max-width: 1200px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  gap: 2rem;
  padding: 0 2rem;
  position: relative;
}

.logo-column {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
}

.college-seal {
  width: 150px;
  height: auto;
  filter: brightness(0) invert(1);
}

.doe-logo {
  width: 120px;
  height: auto;
  filter: brightness(0) invert(1);
}

.info-column {
  padding: 0 1rem;
}

.info-column h2 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  font-weight: normal;
}

.info-column p {
  margin: 0.5rem 0;
  font-size: 1rem;
  line-height: 1.5;
}

.social-icons {
  position: absolute;
  right: 2rem;
  bottom: -1rem;
  display: flex;
  gap: 1rem;
}

.social-icon {
  width: 24px;
  height: 24px;
  filter: brightness(0) invert(1);
}

/* Vertical lines between columns */
.info-column {
  border-left: 1px solid rgba(255, 255, 255, 0.3);
  height: 100%;
}




.socials {
  display: flex;
  justify-content: center;
  gap: 1rem;
  margin-top: 1rem;
}

.socials img {
  width: 24px;
  height: 24px;
}

hr {
  margin: 1rem 0;
  border: none;
  border-top: 1px solid #ddd;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }


  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;
  }


}
</style>