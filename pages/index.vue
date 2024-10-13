<template>
  <div id="app">
    <header :class="{ sticky: isSticky }">
      <img id="logo" src="../assets/img/logo.png" />
      <nav class="mt-5">
        <a href="#Home" @click.prevent="scrollTo('Home')" >Home</a>
        <a href="#aboutme" @click.prevent="scrollTo('aboutme')">about</a>
        <a href="#project" @click.prevent="scrollTo('project')">project</a>
        <a href="#contact" @click.prevent="scrollTo('contact')">contact</a>
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
            Hello, I'm FAJAR ISMAIL, a frontend developer focused on creating responsive user interfaces. I combine
            creativity with technology to deliver effective web solutions.
        </p>
    </div>
    <div class="image-container">
        <img src="../assets/img/fajar.png" alt="Fajar Ismail" />
    </div>
</div>
      <div class="about p-5" id="aboutme">
        <h1 class="ms-5 my-5 text-light">About Me</h1>
        <div class="row text-light">
          <div class="col-lg-4 d-flex justify-content-center py-5">
            <div class="card  rounded-circle" style="width: 18rem; background-color: black">
              <div class="card-body">
                <img class="p-1" src="../assets/img/pr.png" alt="" style="width: 100%; border-radius:100%;" />
              </div>
            </div>
          </div>
          <div class="col-lg-8 d-flex justify-content-center text-light">
            <div class="about-text pt-5 text-light">
          <p>
            Hello! My name is Fajar Ismail, and I am a frontend developer experienced in building engaging and
            responsive web applications. I possess skills in HTML, CSS, and
            JavaScript, along with experience in framework such as Nuxt.js and Vue.js. I truly enjoy the challenge of
            creating intuitive and satisfying user interfaces.
            Additionally, I prioritize good design principles to ensure an optimal user experience. I constantly strive
            to keep up with the latest trends and technologies in web
            development. Outside of coding, I enjoy collaborating with teams and sharing knowledge about best practices
            in development.
          </p>
          <br />
          <p>Thank you for taking the time to get to know me. I look forward to contributing to exciting projects!</p>
        </div>
          </div>
        </div>
        <div class="tools mt-5 pt-5">
          <h1 class="ms-5 my-5 text-light">Tools</h1>
          <div class="row">
            <div class="col-lg-3 p-5">
              <div class="card bg-transparent border-primary">
                <div class="card-bod">
                  <div class="row">
                    <div class="col-4">
                      <img src="../assets/img/html.png" alt="" id="lt">
                    </div>
                    <div class="col-8 mt-4 text-light">
                      <h5>HTML</h5>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-3 p-5">
              <div class="card bg-transparent border-primary">
                <div class="card-bod">
                  <div class="row">
                    <div class="col-4">
                      <img src="../assets/img/css.png" alt="" id="lt">
                    </div>
                    <div class="col-8 mt-4 text-light">
                      <h5>CSS</h5>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-3 p-5">
              <div class="card bg-transparent border-primary">
                <div class="card-bod">
                  <div class="row">
                    <div class="col-4">
                      <img src="../assets/img/js.png" alt="" id="lt">
                    </div>
                    <div class="col-8 mt-4 text-light">
                      <h5>JavaScript</h5>
                    </div>
                  </div>
                </div>
              </div>
            </div>

            <div class="col-lg-3 p-5">
              <div class="card bg-transparent border-primary">
                <div class="card-bod">
                  <div class="row">
                    <div class="col-4">
                      <img src="../assets/img/nx.png" alt="" id="lt">
                    </div>
                    <div class="col-8 mt-4 text-light">
                      <h5>NUXT JS</h5>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-3 p-5">
              <div class="card bg-transparent border-primary">
                <div class="card-bod">
                  <div class="row">
                    <div class="col-4">
                      <img src="../assets/img/v.png" alt="" id="lt">
                    </div>
                    <div class="col-8 mt-4 text-light">
                      <h5>VUE JS</h5>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-3 p-5">
              <div class="card bg-transparent border-primary">
                <div class="card-bod">
                  <div class="row">
                    <div class="col-4">
                      <img src="../assets/img/nd.png" alt="" id="lt">
                    </div>
                    <div class="col-8 mt-4 text-light">
                      <h5>NODE</h5>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-3 p-5">
              <div class="card bg-transparent border-primary">
                <div class="card-bod">
                  <div class="row">
                    <div class="col-4">
                      <img src="../assets/img/b.png" alt="" id="lt">
                    </div>
                    <div class="col-8 mt-4 text-light">
                      <h5>BOOTSTRAP</h5>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-3 p-5">
              <div class="card bg-transparent border-primary">
                <div class="card-bod">
                  <div class="row">
                    <div class="col-4">
                      <img src="../assets/img/t.png" alt="" id="lt">
                    </div>
                    <div class="col-8 mt-4 text-light">
                      <h5>TAILWIND</h5>
                    </div>
                  </div>
                </div>
              </div>
            </div>
            <div class="col-lg-3 p-5">
              <div class="card bg-transparent border-primary">
                <div class="card-bod">
                  <div class="row">
                    <div class="col-4">
                      <img src="../assets/img/p.png" alt="" id="lt">
                    </div>
                    <div class="col-8 mt-4 text-light">
                      <h5>POSTGRESQL</h5>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="project my-5 py-5" id="project">
        <h1 class="ms-5 ps-4 my-5 text-light">Project</h1>
        <div class="row my-5 py-5">
          <div class="col-lg-3 p-5 d-flex justify-content-center">
            <div class="card " style="height: 100%;" id="pr">
              <div class="card-content p-2">
                <img src="../assets/img/ang.jpg" class="card-img-top" alt="..." />
              </div>
            </div>
          </div>
          <div class="col-lg-3 p-5  d-flex justify-content-center">
            <div class="card " style="height: 100%;" id="pr">
              <div class="card-content p-2">
                <img src="../assets/img/cashier.jpg" class="card-img-top" alt="..." />
              </div>
            </div>
          </div>
          <div class="col-lg-3 p-5  d-flex justify-content-center">
            <div class="card" style="height: 100%;" id="pr">
              <div class="card-content p-4">
                <img src="..." class="card-img-top" alt="..." />
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="contact px-5 mx-5 pt-5 mt-5" id="contact">
        <h1 class="d-flex justify-content-center text-light pt-5">Contact me</h1>
        <div class="row justify-content-center align-items-center">
          <div class="col-md-10 col-sm-6 px-5">
            <div class="card my-3 p-2 text-center  bg-transparent border-2 border-white" style="opacity: 80%">
              <form>
                <div class="mb-4 px-5 mt-4">
                  <h3 class="text-light mb-2" style="display: flex; justify-content: start;">Name</h3>
                  <input type="text" class="form-control rounded-2 p-2 bg-transparent text-light"
                    placeholder="Name ......." />
                </div>
                <div class="mb-4 px-5">
                  <h3 class="text-light mb-2" style="display: flex; justify-content: start;">Email</h3>
                  <input type="email" class="form-control rounded-2 p-2 bg-transparent text-light"
                    placeholder="Email ......." />
                </div>
                <div class="mb-4 px-5">
                  <h3 class="text-light mb-2" style="display: flex; justify-content: start;">Message</h3>
                  <textarea name="Message" class="form-control rounded-2 p-2 bg-transparent text-light"
                    placeholder="Message"></textarea>
                </div>
                <div class="mb-4 mx-5 mb-2">
                  <button type="submit" class="btn mb-5 px-5 py-3 form-control" style="background-color: white">
                    <h3>SEND MESSAGE</h3>
                  </button>
                </div>
              </form>
            </div>
          </div>
          <div class="collapse">

          </div>
        </div>
      </div>
      <div class="footer pt-5">
        <hr class="border border-light border-2 my-4" style="width: 100%">
        <div class="row">
          <div class="col-12 col-md-3 my-5 ps-5">
            <h4 class="pb-3">Contact</h4>
            <p>Email: fjarr47@gmail.com</p>
            <p>Phone: +62-857-2386-7299</p>
          </div>
          <div class="col-12 col-md-3 my-5 px-5">
            <h4 class="pb-3">Company</h4>
            <ul>
              <li>WEFRAZ</li>
              <li>CP MAIL</li>
              <li>Spetrum</li>
            </ul>
          </div>
          <div class="col-12 col-md-3 my-5 px-5">
            <ul class="list-inline my-5 text-center">
              <li class="list-inline-item m-3">
                <i class="bi bi-github"></i>
              </li>
              <li class="list-inline-item m-3">
                <i class="bi bi-twitter-x"></i>
              </li>
              <li class="list-inline-item m-3">
                <i class="bi bi-instagram"></i>
              </li>
              <li class="list-inline-item m-3">
                <i class="bi bi-linkedin"></i>
              </li>
            </ul>
          </div>
          <div class="col-12 col-md-3 my-5 px-5">
            <h4 class="pb-3">Random Quote</h4>
            <p>"Every mistake is a teacher. Don't be afraid to fail, as it is a part of your journey."</p>
            <hr class="mt-4">
            <div class="cr mt-4">copyright@fajarismail-2024</div>
          </div>
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
@import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css");
h5{
  font-size: 13px;
}
.text-content {
    max-width: 600px;
}

h1 {
    font-size: 4vw;
}

.developer-title {
    font-size: 2.5vw;
    margin: 10px 0;
}

p {
    font-size: 1.5vw;
}

.image-container img {
    width: 100%;
    height: auto;
}
.footer {
  padding-top: 5rem;
}

.footer h4 {
  font-size: 1.5rem;
}

.footer p {
  font-size: 1rem;
}

.footer .navbar-nav i {
  font-size: 1.5rem;
  margin: 0 10px;
}
.list-inline-item i {
    font-size: 1.5rem; 
  }
  .card-title {
  font-size: 1.5rem;
}

.card-text {
  font-size: 1rem;
}


@media (max-width: 768px) {
  h1 {
        font-size: 30px;
    }

    .developer-title {
        font-size: 10px;
    }

    p {
        font-size: 1px;
    }
  
  .card-text, .about-text p {
    font-size: 1rem;
  }
  .footer {
    padding-top: 2rem;
  }

  .footer h4 {
    font-size: 1.2rem;
  }
  .footer p {
    font-size: 0.9rem;
  }

  .footer .navbar-nav i {
    font-size: 1.2rem;
  }
  .list-inline-item i {
    font-size: 1rem; 
  }
  .tools h5 {
    font-size: 1rem;
  }
}

@media (max-width: 576px) {
  h1 {
        font-size: 30px;
    }

    .developer-title {
        font-size: 10px;
    }

    p {
        font-size: 1px;
    }

    .image-container img {
        width: 80%;
        height: auto;
    }
  .card-title {
    font-size: 1rem;
  }

  .card-text, .about-text p {
    font-size: 0.9rem;
  }
  .footer {
    padding: 1rem;
  }

  .footer h4 {
    font-size: 1rem;
  }

  .footer p {
    font-size: 0.8rem;
  }

  .footer .navbar-nav {
    flex-direction: column;
    align-items: center;
  }
  .list-inline-item i {
    font-size: 0.8rem; 
  }
  .tools h5 {
    font-size: 0.9rem;
  }
}

#lt {
  margin: 10%;
  height: 50px;
  width: 50px;
}

#pr {
  background-color: #0f0f0f;
}

i {
  font-size: 50px;
  margin: 10%;
}

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
