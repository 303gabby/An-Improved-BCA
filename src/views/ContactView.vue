<template>
  <div class="contact">
    <h1 class="main-title">Contact Us</h1>
    
    <div class="campus-image">
      <img src="@/assets/campus.png" alt="Image of Brooklyn Colleges Campus." width="1267" height="421">
    </div>
    
    <div class="description">
      <h2>Brooklyn College Academy is a dual-sited school, where the 9-10th grade is located 
        at 350 Coney Island Avenue, and the 11-12th grade is housed in James Hall at Brooklyn College. 
        This setup provides younger students with a dedicated space for their foundational years, while 
        upperclassmen benefit from being immersed in a college campus environment.</h2>
    </div>

    <div class="locations-container">
      <div class="location">
        <h1>Brooklyn College Academy High School</h1>
        <div class="contact-info">
          <p>Address: 350 Coney Island Ave. Brooklyn, NY 11218</p>
          <p>Email: bcaconnection@brooklyncollegeacademy.com</p>
          <p>Phone: (718) 853-6184</p>
          <p>Fax: (718) 853-6356</p>
        </div>
      </div>

      <div class="location">
        <h1>Brooklyn College Campus</h1>
        <div class="contact-info">
          <p>Address: 2900 Bedford Avenue James Hall 1311, Brooklyn, NY 11210</p>
          <p>Email: bcaconnection@brooklyncollegeacademy.com</p>
          <p>Phone: (718) 951-5941</p>
          <p>Fax: (718) 951-4441</p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.contact {
  min-height: 100vh;
  padding: 2rem;
  max-width: 1440px;
  margin: 0 auto;
}

.main-title {
  text-align: center;
  margin-bottom: 2rem;
  font-size: 2rem;
}

.campus-image {
  width: 100%;
  margin-bottom: 2rem;
  overflow: hidden;
}

.campus-image img {
  width: 100%;
  height: auto;
  object-fit: cover;
}

.description {
  margin-bottom: 3rem;
  padding: 0 1rem;
}

.description h2 {
  font-size: 1.2rem;
  line-height: 1.6;
  font-weight: normal;
  text-align: justify;
}

.locations-container {
  display: grid;
  gap: 2rem;
  margin-top: 2rem;
}

.location {
  padding: 1.5rem;
  background-color: #f8f8f8;
  border-radius: 8px;
}

.location h1 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  color: #74218A;
}

.contact-info p {
  margin: 0.5rem 0;
  font-size: 1rem;
  line-height: 1.5;
}

/* Responsive Design */
@media (min-width: 768px) {
  .locations-container {
    grid-template-columns: 1fr 1fr;
  }
}

@media (min-width: 1024px) {
  .contact {
    padding: 3rem;
  }

  .description h2 {
    font-size: 1.3rem;
  }

  .location {
    transition: transform 0.2s ease;
  }

  .location:hover {
    transform: translateY(-5px);
  }
}
</style>