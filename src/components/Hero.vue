<template>
  <section id="hero">
    <div class="container_hero">
      <div class="box">
        <img src="@/assets/foto.png" class="foto_perfil" data-aos="fade-zoom-in" data-aos-easing="ease-in-back"
    data-aos-delay="300"
    data-aos-offset="0" />
        <div class="title">
          <span class="block"></span>
          <h1>David Font<span></span></h1>
        </div>

        <div class="role">
          <div class="block"></div>
          <p>Front End Dev / Maquetador Web</p>
        </div>

        <div class="row col-8 offset-2 mt-5" data-aos="fade-right" data-aos-delay="300">
          <div class="col-sm">
            <img src="@/assets/linkedin.png" @click="goTo('linkedin')" class="mt-3 float-right" height="30" />
          </div>
          <div class="col-sm">
            <img src="@/assets/instagram.png" @click="goTo('instagram')" class="mt-3 float-right" height="30" />
          </div>
        </div>

      </div>
      <div class="wave"></div>
    </div>
  </section>
</template>

<script>
export default{
    name: 'HeroComponent',
    methods: {
    goTo (value) {
      switch(value) {
        case 'linkedin': 
          window.open('https://www.linkedin.com/in/david-font-7508a1221/');
          break;
        case 'instagram': 
          window.open('https://www.instagram.com/dfont93');
          break;
      }
    }
  }
}
</script>


<style lang="scss" scoped>

/****************************
        ANIMACION WAVE 
*****************************/

img {
  cursor: pointer;
}

section .wave {
  position: absolute;
  width: 100%;
  height: 143px;
  bottom: 0;
  left: 0;
  background: url(../assets/wave.png);
  animation: animate 10s linear infinite;
}

section .wave:before {
  content: "";
  width: 100%;
  height: 143px;
  background: url(../assets/wave.png);
  position: absolute;
  top: 0;
  left: 0;
  opacity: 0.4;

  animation: animate-reverse 10s linear infinite;
}

@keyframes animate {
  0% {
    background-position: 0px;
  }
  100% {
    background-position: 1360px;
  }
}

@keyframes animate-reverse {
  0% {
    background-position: 1360px;
  }
  100% {
    background-position: 0;
  }
}

/****************************
  ANIMACION NOMBRE Y TRABAJO 
*****************************/

.section {
  width: 100%;
  margin: 0;
  padding: 0;
}
.container_hero {
  background: url(../assets/Pano_cueva_roja_xs.jpg) top center no-repeat;
  width: 100%;
  overflow: hidden;
  height: 1050px;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
}

.foto_perfil {
  width: 246px;
  height: 240px;
  margin-left: 1px;
  margin-top: 1px;
  border-radius: 250px;
}

.box {
  width: 250px;
  height: 250px;
  position: relative;
  display: flex;
  justify-content: center;
  flex-direction: column;

  .title {
    width: 100%;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    height: 50px;
    margin-top: 50px;

    .block {
      width: 0%;
      height: inherit;
      background: #ffb510;
      position: absolute;
      animation: mainBlock 2s cubic-bezier(0.74, 0.06, 0.4, 0.92) forwards;
      display: flex;
    }

    h1 {
      font-family: "Poppins";
      color: #fff;
      font-size: 50px;
      -webkit-animation: mainFadeIn 2s forwards;
      -o-animation: mainFadeIn 2s forwards;
      animation: mainFadeIn 2s forwards;
      animation-delay: 1.6s;
      opacity: 0;
      display: flex;
      align-items: baseline;
      position: relative;

      span {
        width: 0px;
        height: 0px;
        -webkit-border-radius: 50%;
        -moz-border-radius: 50%;
        border-radius: 50%;

        background: #ffb510;
        -webkit-animation: load 0.6s cubic-bezier(0.74, 0.06, 0.4, 0.92)
          forwards;
        animation: popIn 0.8s cubic-bezier(0.74, 0.06, 0.4, 0.92) forwards;
        animation-delay: 2s;
        margin-left: 5px;
        margin-top: -10px;
        position: absolute;
        bottom: 13px;
        right: -12px;
      }
    }
  }

  .role {
    width: 100%;
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 30px;
    margin-top: 30px;

    .block {
      width: 0%;
      height: inherit;
      background: #e91e63;
      position: absolute;
      animation: secBlock 2s cubic-bezier(0.74, 0.06, 0.4, 0.92) forwards;
      animation-delay: 2s;
      display: flex;
    }

    p {
      animation: secFadeIn 2s forwards;
      animation-delay: 3.2s;
      opacity: 0;
      font-weight: 400;
      font-family: "Lato";
      color: #ffffff;
      font-size: 16px;
      text-transform: uppercase;
      letter-spacing: 5px;
    }
  }
}

@keyframes mainBlock {
  0% {
    width: 0%;
    left: 0;
  }
  50% {
    width: 100%;
    left: 0;
  }
  100% {
    width: 0;
    left: 100%;
  }
}

@keyframes secBlock {
  0% {
    width: 0%;
    left: 0;
  }
  50% {
    width: 100%;
    left: 0;
  }
  100% {
    width: 0;
    left: 100%;
  }
}

@keyframes mainFadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

@keyframes popIn {
  0% {
    width: 0px;
    height: 0px;
    background: #e9d856;
    border: 0px solid #ddd;
    opacity: 0;
  }
  50% {
    width: 10px;
    height: 10px;
    background: #e9d856;
    opacity: 1;
    bottom: 45px;
  }
  65% {
    width: 7px;
    height: 7px;
    bottom: 0px;
    width: 15px;
  }
  80% {
    width: 10px;
    height: 10px;
    bottom: 20px;
  }
  100% {
    width: 7px;
    height: 7px;
    background: #e9d856;
    border: 0px solid #222;
    bottom: 13px;
  }
}

@keyframes secFadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 0.5;
  }
}
</style>

