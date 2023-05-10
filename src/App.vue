<template>
  <div id="app">
    <header>
      <div class="title">
        <img src="./assets/logo.png" alt="Logo" class="logo" />
        <h1 style="margin: 0;">Bridgeby Tradings Ltd</h1>
      </div>
      <div>
        <h3 style="margin: 0.5rem;">Established 2023</h3>
      </div>
    </header>
    <div class="container">
      <div class="about">
        <p>Bridgeby Tradings Ltd is a holding company established in 2023 that deals primarily in the building and running of e-commerce sites. It also deals with physical sales in the form of pop-up shops in the London (UK) area.</p>
      </div>
    
      <div class="main">
        <hr class="divider" />
        <div>
          <div class="content">
            <div class="image-div">
              <img src="./assets/image.jpg" alt="Image" class="image" />
            </div>
            <div class="text-div">
              <p>Bridgeby Tradings Ltd is currently seeking suppliers of</p>
              <ul>
                <li>Musical instruments and accessories</li>
                <li></li>
              </ul>
            </div>
          </div>
          <hr class="divider" />
          <div style="text-align: center;">
              <address> 
                  <a href="mailto:info@bridgebytradings.co.uk" class="contact">Contact
                      <img src="./assets/email.png" class="email-icon">
                  </a>
              </address>
          </div>
        </div>
      </div>
  </div>
  </div>
</template>

<script>
export default {
  name: "App",
};
</script>

<style scoped>


#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  background-color: #0f0067;
  color: #fff; 
}

header {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: #f1f1f1;
  padding: 20px;
  color: #000;
}

.container{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: calc(100% - 120px);
  width: 90%;
  margin: 0 auto;
}

.about {
  width: 70%;
  text-align: center;
  margin: 2rem;
  color: #fff;
}

.main {
  width: 100%
}

.logo {
  width: 50px;
  height: 50px;
  margin-right: 10px;
}

.title {
  display: flex;
  justify-content: center;
  align-items: center;
}

.divider {
  border: 1px solid #fffefe;
  margin: 2rem 0;
}

.content {
  display: flex;
  justify-content: space-around;
}

.image-div,
.text-div {
  border: 1px solid #fefefe;
  border-radius: 10px;
  padding: 20px;
  width: 300px;
}

.image {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.contact {
  font-size: 1.5rem;
  text-decoration: none;
  text-align: center;
  color: #fff;
  font-style: normal;

}

.email-icon {
  width: 50px;
  height: 50px;
  display: block;
  filter:invert(100%);
  margin: 0.75rem auto;
  transition: scale 0.3s ease;
  }
.email-icon:hover {
    scale: 1.3;
  }

@media only screen and (max-width: 768px) {
  .content {
    flex-direction: column;
    align-items: center;
  }
  .text-div {
    margin-top: 20px;
  }
  .title {
    flex-direction: column;
  }
}
</style>
