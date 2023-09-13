<template>
    <section class="services-container col-8 offset-2 pb-5" data-aos="fade-zoom-in"
     data-aos-easing="ease-in-back"
     data-aos-delay="300"
     data-aos-offset="0">
      <div class="row justify-content-center w-80 p-0 m-0">

            <div class="col-10 col-xxl-12 services_title p-3 pb-5">
            <hr width="50" size="4" class="text-white" />
            <span class="text-white">Servicios</span>
            </div>

            <div class="row row-cols-1 row-cols-md-4  col-10 offset-1 fondo_card g-4">
                <div class="col" v-for="item in servicios" :key="item.id">
                    <div class="card h-100">
                    <img src="@/assets/approval.png" class="card-img-top" height="50" width="50" alt="...">
                    <div class="card-body">
                        <h5 class="card-title mt-2 text-center text-white">{{ item.title }}</h5>
                        <p class="card-text text-center text-white">{{ item.text }}</p>
                    </div>
                    </div>
                </div>
            </div>
            
      </div>
    </section>   
</template>

<script>
export default {
  name: 'ServiciosComp',
  setup () {
    let servicios = [
        { id: 1, title: 'HTML', text: 'Básico+' },
        { id: 2, title: 'CSS', text: 'Básico+' },
        { id: 3, title: 'JavaScript', text: 'Básico' },
        { id: 4, title: 'Tailwind', text: 'Básico+' },
        { id: 5, title: 'Vue', text: 'Intermedio' },
        { id: 6, title: 'Vuex', text: 'Básico' },
        { id: 7, title: 'Firebase', text: 'Intermedio' },
        { id: 8, title: 'Flutter', text: 'Básico+' },
        { id: 9, title: 'Dart', text: 'Básico+' },
        { id: 10, title: 'React', text: 'Intermedio' },
        { id: 11, title: 'Git', text: 'Básico' },
        { id: 12, title: 'Figma/XD', text: 'Básico' }
    ]

    return {
        servicios
    }
  }
}
</script>

<style lang="scss" scoped>
* {
    font-family: Overlock;
}
/****************************
          SERVICIOS
*****************************/
section .services-container {
  display: flex;
  width: 80%;
  height: 80px;
  margin: 0px;
  overflow: hidden;
}

.services_title {
  display: flex;
  grid-row: auto;
  align-items: center;
  margin-top: 100px;
}

section .services_title span {
  font-size: 26px;
  font-family: Overlock;
  margin-left: 20px;
}

.services_box {
height: 400px;
left: 525px;
top: 541px;
background: #151C26;
border-radius: 15px;
}

.fondo_card, .card {
    background: #151C26;
    border: 0px;
    border-radius: 15px;
}

.card img {
    width: 25px;
    height: 25px;
    display: block;
    margin: 0 auto;
}

.card-img {
    height: 30px;
    width: 30px;
}
.card-body {
    padding-top: 3px;
}

.card-title, .card-text {
    text-align: left;
}

.card-title {
    margin-bottom: 3px;
}

.card-text {
    font-size: 12px;
}
</style>
