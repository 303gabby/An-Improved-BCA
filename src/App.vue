<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'

</script>

<template>
  <header>

    <div class="wrapper">
      

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/academics">Academics</RouterLink>
        <RouterLink to="/admissions">Admission</RouterLink>
        <img alt="Vue logo" class="logo" src="@/assets/Brooklyn_College_Seal.svg" width="125" height="125" />
        <RouterLink to="/students">Students</RouterLink>
        <RouterLink to="/parents">Parents</RouterLink>
        <RouterLink to="/contact">Contact Us</RouterLink>
       
      </nav>
    </div>
  </header>

  <footer>

    <div id = "main footer div"> 
      <div id = "footer img">
        <img src="@/assets/Brooklyn_College_Seal.svg" alt="Seal of Brooklyn College">
      </div>
      <hr>

      <div id = "main site">
       <h1>Main Site (Grades 9-10) </h1>
       <p>350 Coney Island Ave, Brooklyn NY 11218</p>
       <p>Email: bcaconnection@brooklyncollegeacademy.com</p>
       <p>Phone:  (718) 853 6184</p>
       <p>Fax:       (718) 853 6356</p>
      </div>
      <hr>
      <div id = "Campus site">
       <h1>Campus Site (Grades 11-12)</h1>
       <p>2900 Bedford  Ave, Brooklyn NY 11230</p>
       <p>Email: bcaconnection@brooklyncollegeacademy.com</p>
       <p>Phone:  (718) 951 5941</p>
       <p>Fax:       (718) 951 4441</p>
      </div>
      <hr>
      <div id = "socials">
        <a href="mailto:bcaconnection@brooklyncollegeacademy.com">
          <img src = "@/assets/envelope.svg" alt="clickable image of envelope for email contact">
         </a>
         <a href="https://www.instagram.com/bca.world/">
          <img src = "@/assets/instagram-logo.svg" alt="clickable image of instagram icon to navigate to instagram">
         </a>
         
      </div>
    </div>
  </footer>

  <RouterView />
</template>

<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
  background-color: #FFFF;
 
}

nav a.router-link-exact-active {
  color:  #74218A;
}

nav a.router-link-exact-active:hover {
  background-color: #74218A;
  color: #FFFF;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}
</style>
