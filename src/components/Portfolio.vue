<template>
     <section class="about-container col-8 offset-2 pb-5">
      <div class="row justify-content-center p-0 m-0">
        <div class="col-10 col-xxl-12 about_title p-3 pb-5">
          <hr width="50" size="4" class="text-white" />
          <span class="text-white">Portfolio</span>
        </div>

        <div class="row row-cols-1 row-cols-md-3 g-4 mt-0" data-aos="flip-left"
              data-aos-easing="ease-out-cubic"
              data-aos-duration="2000">
          <div class="col-xs-12 col-md-12 col-lg-6">
            <div class="card h-200" @click="goTo('Gestió')">
              <img src="@/assets/tr_gestion.png" class="card-img-top" alt="...">
              <div class="card-body">
                <h5 class="card_title mb-1">Gestió Taller Radio</h5>
                <p class="card_text">Vue + Vuex + Vuetify + Firebase</p>
              </div>
            </div>
          </div>
          <div class="col-xs-12 col-md-12 col-lg-6" data-aos="flip-left"
                data-aos-easing="ease-out-cubic"
                data-aos-duration="2000">
            <div class="card h-200" @click="goTo('Curriculum')">
              <img src="@/assets/cv_web.png" class="card-img-top" alt="...">
              <div class="card-body">
                <h5 class="card_title mb-1">Curriculum Web</h5>
                <p class="card_text">HTML + CSS + BootStrap + Vue</p>
                <!-- <a href="https://vibrant-engelbart-1f6c0c.netlify.app/" class="btn-proyecto">Ir</a>-->
              </div>
            </div>
          </div>

          <div class="col-xs-12 col-md-12 col-lg-6" data-aos="flip-left"
            data-aos-easing="ease-out-cubic"
            data-aos-duration="2000">
            <div class="card h-200" @click="goTo('Restaurant')">
              <img src="@/assets/restaurant.png" class="card-img-top" alt="...">
              <div class="card-body">
                <h5 class="card_title mb-1">Restaurante</h5>
                <p class="card_text">HTML + CSS + BootStrap + Vue</p>
                <!-- <a href="https://vibrant-engelbart-1f6c0c.netlify.app/" class="btn-proyecto">Ir</a>-->
              </div>
            </div>
          </div>

          <div class="col-xs-12 col-md-12 col-lg-6" data-aos="flip-left"
            data-aos-easing="ease-out-cubic"
            data-aos-duration="2000">
            <div class="card h-180" @click="goTo('Notes')">
              <img src="@/assets/notes.png" class="card-img-top" alt="...">
              <div class="card-body">
                <h5 class="card_title mb-1">Notes Firestore</h5>
                <p class="card_text">Flutter + Firestore + Cloud Storage</p>
                <!-- <a href="https://vibrant-engelbart-1f6c0c.netlify.app/" class="btn-proyecto">Ir</a>-->
              </div>
            </div>
          </div>

          <div class="col-xs-12 col-md-12 col-lg-6" data-aos="flip-left"
            data-aos-easing="ease-out-cubic"
            data-aos-duration="2000">
            <div class="card h-180" @click="goTo('Recipes')">
              <img src="@/assets/recipes.png" class="card-img-top" alt="...">
              <div class="card-body">
                <h5 class="card_title mb-1">Recipes UI</h5>
                <p class="card_text">Flutter </p>
                <!-- <a href="https://vibrant-engelbart-1f6c0c.netlify.app/" class="btn-proyecto">Ir</a>-->
              </div>
            </div>
          </div>

          <div class="col-xs-12 col-md-12 col-lg-6" data-aos="flip-left"
            data-aos-easing="ease-out-cubic"
            data-aos-duration="2000">
            <div class="card h-180" @click="goTo('Auth')">
              <img src="@/assets/auth_bloc_firestore.png" class="card-img-top" alt="...">
              <div class="card-body">
                <h5 class="card_title mb-1">Boilerplate BLOC Auth Firestore</h5>
                <p class="card_text">Flutter + Auth Firebase + BLOC </p>
                <!-- <a href="https://vibrant-engelbart-1f6c0c.netlify.app/" class="btn-proyecto">Ir</a>-->
              </div>
            </div>
          </div>

          <div class="col-xs-12 col-md-12 col-lg-6" data-aos="flip-left"
            data-aos-easing="ease-out-cubic"
            data-aos-duration="2000">
            <div class="card h-180" @click="goTo('Crud')">
              <img src="@/assets/auth_crud_bloc_firestore.png" class="card-img-top" alt="...">
              <div class="card-body">
                <h5 class="card_title mb-1">Boilerplate BLOC Auth & CRUD Firestore</h5>
                <p class="card_text">Flutter + Auth Firebase + Firestore DB + BLOC </p>
                <!-- <a href="https://vibrant-engelbart-1f6c0c.netlify.app/" class="btn-proyecto">Ir</a>-->
              </div>
            </div>
          </div>   
          
          <div class="col-xs-12 col-md-12 col-lg-6" data-aos="flip-left"
            data-aos-easing="ease-out-cubic"
            data-aos-duration="2000">
            <div class="card h-180" @click="goTo('Mern')">
              <img src="@/assets/mern_fullstack.png" class="card-img-top" alt="...">
              <div class="card-body">
                <h5 class="card_title mb-1">MERN Full Stack Recipe App</h5>
                <p class="card_text">React + Tailwind + Express + Node </p>
                <!-- <a href="https://vibrant-engelbart-1f6c0c.netlify.app/" class="btn-proyecto">Ir</a>-->
              </div>
            </div>
          </div>

          <div class="col-xs-12 col-md-12 col-lg-6" data-aos="flip-left"
            data-aos-easing="ease-out-cubic"
            data-aos-duration="2000">
            <div class="card h-180" @click="goTo('Mern')">
              <img src="@/assets/blog_frontend_miniatura.png" class="card-img-top" alt="...">
              <div class="card-body">
                <h5 class="card_title mb-1">MERN Full Stack Blog App</h5>
                <p class="card_text">React + Tailwind + MongoDB + Express + Node </p>
                <!-- <a href="https://vibrant-engelbart-1f6c0c.netlify.app/" class="btn-proyecto">Ir</a>-->
              </div>
            </div>
          </div>   

        </div>
      </div>
    </section>  
</template>

<script>
export default {
  name: 'PortfolioComp',
  methods: {
    goTo (value) {
      switch(value) {
        case 'Gestió': 
          window.open('https://linksta.cc/@dfont93');
          break;
        case 'Curriculum': 
          window.open('https://linksta.cc/@dfont93');
          break;
        case 'Restaurant': 
          window.open('https://linksta.cc/@dfont93');
          break;
        case 'Notes': 
          window.open('https://linksta.cc/@dfont93');
          break;
        case 'Recipes': 
          window.open('https://linksta.cc/@dfont93');
          break;
        case 'Auth': 
          window.open('https://linksta.cc/@dfont93');
          break;
        case 'Crud': 
          window.open('https://linksta.cc/@dfont93');
          break;
        case 'Mern': 
          window.open('https://linksta.cc/@dfont93');
          break;
      }
    }
  }
}
</script>

<style lang="scss" scoped>

/****************************
            ABOUT
*****************************/
section .about-container {
  display: flex;
  width: 80%;
  height: 80px;
  margin: 0px;
}

.about_title {
  display: flex;
  grid-row: auto;
  align-items: center;
  margin-top: 100px;
}

section .about_title span {
  font-size: 26px;
  font-family: Overlock;
  margin-left: 20px;
}

.card {
  position: relative;
  border: 0px;
  padding: 0px;
  background-color: transparent;
  cursor: pointer;
  min-width: 250px;
}

.card:hover {
  position: relative;
  border: 0px;
  padding: 0px;
  background: rgba(255, 255, 255, 0.6);
  cursor: pointer;
}


.card-img-overlay {
  align-items: end;
}

.card-img-top {
  border-radius: 20px;
}

.card_title {
  font-family: Overlock;
  font-size:  22px;
  font-weight: 600;
  color: white;
}

.card_text {
  font-size: 13px;
  color: rgb(211, 211, 211);
  opacity: 1 !important;
}

.card-body {
  position: absolute;                 
  bottom:0;                         
  left:0;  
  width: 100%;
  background: rgba(0,0,0, .3);
}


/* MEDIA QUERIES 
@media screen and (max-width: 1285px) {
  .cards-wrapper {
    grid-template-columns: 1fr 1fr;
  }
}

@media screen and (max-width: 900px) {
  .cards-wrapper {
    grid-template-columns: 1fr;
  }
  .info {
    justify-content: center;
  }
  .card-grid-space .num {
    margin-left: 0;
    text-align: center;
  }
}

@media screen and (max-width: 500px) {
  .cards-wrapper {
    padding: 4rem 2rem;
  }
  .card {
    max-width: calc(100vw - 4rem);
  }
}

@media screen and (max-width: 450px) {
  .info {
    display: block;
    text-align: center;
  }
  .info h1 {
    margin: 0;
  }
}*/


</style>