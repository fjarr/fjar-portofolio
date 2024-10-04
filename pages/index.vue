<template>
  <div id="app">
    <header :class="{ sticky: isSticky }">
      <img id="logo" src="../assets/img/logo.png" />
      <nav class="mt-5">
        <a href="#Home" @click.prevent="scrollTo('Home')">Home</a>
        <a href="#aboutme" @click.prevent="scrollTo('aboutme')">about</a>
        <a href="#space" @click.prevent="scrollTo('space')">Space</a>
        <a href="#future" @click.prevent="scrollTo('future')">Future</a>
        <button @click="toggleMenu" id="openmenu">
          <span></span>
          <span></span>
        </button>
      </nav>
    </header>
    <div id="page" :class="{ menuopen: menuOpen }">
      <div class="container" id="Home">
        <div class="text-content">
          <h1>FRONTEND</h1>
          <div class="developer-title">developer</div>
          <p>
            Hello, I'm FAJAR ISMAIL, a frontend developer focused on creating responsive user interfaces. I combine creativity with technology to deliver effective web solutions.
          </p>
        </div>
        <div class="image-container">
          <img src="../assets/img/fajar.png" alt="Fajar Ismail" />
        </div>
      </div>
      <div class="about p-5" id="aboutme">
        <h1 class="ms-5 my-5 text-light">About Me</h1>
        <div class="row text-light">
          <div class="col-4 d-flex justify-content-center">
            <div class="card border-primary" style="width: 18rem; background-color: black">
              <div class="card-body">
                <h5 class="card-title">Card title</h5>
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
              </div>
            </div>
          </div>
          <div class="col-4 d-flex justify-content-center py-5">
            <div class="card border-primary rounded-circle" style="width: 18rem; background-color: black">
              <div class="card-body">
                <img class="p-1" src="../assets/img/pr.jpeg" alt="" style="width: 100%; border-radius: 100%" />
              </div>
            </div>
          </div>
          <div class="col-4 d-flex justify-content-center text-light">
            <div class="card border-primary" style="width: 18rem; background-color: black">
              <div class="card-body">
                <h5 class="card-title text-light">Card title</h5>
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
              </div>
            </div>
          </div>
        </div>
        <div class="about-text p-5 text-center mx-5 mt-5 text-light">
          <p>
            Hello! My name is Fajar Ismail, and I am a frontend developer experienced in building engaging and responsive web applications. I possess skills in HTML, CSS, and
            JavaScript, along with experience in framework such as Nuxt.js and Vue.js. I truly enjoy the challenge of creating intuitive and satisfying user interfaces.
            Additionally, I prioritize good design principles to ensure an optimal user experience. I constantly strive to keep up with the latest trends and technologies in web
            development. Outside of coding, I enjoy collaborating with teams and sharing knowledge about best practices in development.
          </p>
          <br />
          <p>Thank you for taking the time to get to know me. I look forward to contributing to exciting projects!</p>
        </div>
      </div>
    </div>
  </div>
  <div class="project my-5 py-5" style="height: 400px;">
    <h1 class="d-flex justify-content-center">Project</h1>
    <div class="row my-5 py-5">
      <div class="col-6 d-flex justify-content-center">
        <div class="card" style="width:  25rem;height: 12rem;">
          <img src="..." class="card-img-top" alt="..." />
        </div>
      </div>
      <div class="col-6 d-flex justify-content-center">
        <div class="card" style="width:  25rem ;height: 12rem;">
          <img src="..." class="card-img-top" alt="..." />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isSticky: false,
      menuOpen: false,
    };
  },
  methods: {
    handleScroll() {
      this.isSticky = window.scrollY >= 100;
    },
    scrollTo(id) {
      const targetElement = document.getElementById(id);
      if (targetElement) {
        targetElement.scrollIntoView({ behavior: 'smooth' });
        this.menuOpen = false;
      }
    },
    toggleMenu() {
      this.menuOpen = !this.menuOpen;
      if (this.menuOpen) {
        this.isSticky = false;
      }
    },
  },
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
  },
  beforeDestroy() {
    window.removeEventListener('scroll', this.handleScroll);
  },
};
</script>

<style scoped>
#app {
  background-color: black;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.text-content {
  color: white;
  margin-top: 25%;
  margin-bottom: 10%;
}

.image-container {
  margin-top: 25%;
  margin-bottom: 10%;
}

#Home {
  margin-left: 10%;
}

.container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 80%;
}

.text-content {
  max-width: 50%;
}

h1 {
  font-weight: bold;
}

.developer-title {
  font-size: 2rem;
  margin-top: 0.5rem;
  margin-bottom: 1.5rem;
}

p {
  font-size: 1.2rem;
  line-height: 1.5;
}

body {
  line-height: 1.6;
  background: #000;
  font-size: 18px;
  font-weight: 400;
  font-family: '-apple-system', 'BlinkMacSystemFont', 'Roboto', 'Helvetica Neue', sans-serif !important;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

body.stop {
  overflow: hidden;
}

#page {
  position: relative;
  transition: 1s all ease-in-out;
}

#page.menuopen {
  opacity: 0.6;
  filter: blur(20px);
  transform: scale(1.2);
}

section {
  display: flex;
  min-height: 100vh;
  padding: 50px;
  justify-content: center;
  align-items: center;
  background: #222;
  color: #fff;
  position: relative;
}

section:after {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  background: #000;
  opacity: 0.5;
  height: 100%;
  width: 100%;
}

section h1 {
  font-size: 120px;
  margin: 0;
  z-index: 2;
  position: relative;
}

header {
  z-index: 99999;
  position: relative;
}

header #logo {
  position: fixed;
  top: 30px;
  left: 0;
  right: 0;
  width: 100px;
  height: auto;
  margin: auto;
  opacity: 1;
  transition: 0.3s all cubic-bezier(0.075, 0.82, 0.165, 1) 0.6s;
}

header nav {
  display: flex;
  flex-wrap: wrap;
  height: 100px;
  justify-content: center;
  align-items: center;
  padding: 0 20px;
  position: fixed;
  left: 0;
  right: 0;
  max-width: 90%;
  margin: 0 auto;
  top: 120px;
  background-color: rgba(255, 255, 255, 0.05);
  border-radius: 200px;
  z-index: 9;
  backdrop-filter: blur(5px);
  border: 1px solid rgba(255, 255, 255, 0.06);
  transition: 1s all cubic-bezier(0.075, 0.82, 0.165, 1) 0.2s;
}

header nav a {
  color: #fff;
  text-decoration: none;
  font-weight: 700;
  display: block;
  padding: 10px 20px;
  line-height: 1;
  font-size: 15px;
  letter-spacing: 2px;
  text-transform: lowercase;
  transition: 0.3s all cubic-bezier(0.075, 0.82, 0.165, 1) 0.6s;
}

header nav button {
  background: rgba(0, 0, 0, 0.3);
  backdrop-filter: blur(5px);
  border: 1px solid rgba(255, 255, 255, 0.1);
  position: absolute;
  z-index: 99;
  left: 0;
  margin: auto;
  right: 0;
  top: 0;
  bottom: 0;
  width: 60px;
  height: 60px;
  border-radius: 100%;
  outline: 0;
  border: 0;
  cursor: pointer;
  transition: 0.3s all cubic-bezier(0.075, 0.82, 0.165, 1) 0.2s;
  transform: scale(0);
}

header nav button span {
  width: 40%;
  background: #fff;
  height: 2px;
  display: block;
  margin: 5px auto;
  transform: scaleX(0);
  transition: 0.6s transform cubic-bezier(0.075, 0.82, 0.165, 1) 0s, 0.3s margin ease-in 0s;
}

header nav button:hover {
  border-color: rgba(255, 255, 255, 0.5);
}

header nav button:hover span {
  margin: 10px auto;
}

header.sticky #logo {
  top: 0;
  transform: scale(0.8);
  opacity: 0;
  transition-delay: 0.5s;
}

header.sticky nav {
  top: 20px;
  padding: 0;
  width: 90px;
  height: 90px;
  transition-delay: 0.5s;
}

header.sticky nav button {
  transform: scale(1);
  transition-delay: 0.6s;
}

header.sticky nav button span {
  transform: scaleX(1);
  transition: 0.6s transform cubic-bezier(0.075, 0.82, 0.165, 1) 0.8s, 0.3s margin ease-in 0s;
}

header.sticky nav a {
  padding: 0;
  opacity: 0;
  letter-spacing: 0px;
  transform: scale(0.3);
  transition-delay: 0.2s;
}
</style>
