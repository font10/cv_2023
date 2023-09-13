<template>
    <section class="trabajo-container col-8 offset-2 pb-5">
      <div class="col-10 col-xxl-12 trabajo_title p-3 pb-5">
          <hr width="50" size="4" class="text-white" />
          <span class="text-white">Estudios</span>
      </div>
  
      <div class="row row-cols-1 row-cols-md-2 g-4 mt-0">
        <div class="col" v-for="item in estudios" :key="item.id">
          <div class="card h-200" :data-aos="item.aos" 
       data-aos-anchor-placement="bottom-bottom" >
            <div class="card-body">
              <span class="card_year">{{ item.ano }}</span>
              <h5 class="card-title text-white mb-0 mt-3">{{ item.title }}</h5>
              <p class="card-text text-white">{{ item.text }}</p>
            </div>
          </div>
        </div>
      </div>
      
    </section>
  </template>
  
  <script>
  export default {
    name: 'EstudiosComponent',
    setup () {
      let estudios = [
          { id: 1, ano: '2005-2009', title: 'ESO', text: 'La Salle', aos: 'fade-up' },
          { id: 2, ano: '2009-2011', title: 'CFGM SMX', text: 'IES Rafael Campalans', aos: 'fade-up' },
          { id: 3, ano: '2011-2012', title: 'Curso Puente', text: 'IES Santa Coloma de Farners', aos: 'fade-up' },
          { id: 4, ano: '2012-2014', title: 'CFGS DAM', text: 'IES Rafael Campalans', aos: 'fade-up' },
          { id: 5, ano: '2017-2018', title: 'CFGS DAW', text: 'IES Rafael Campalans', aos: 'fade-up' },
          { id: 6, ano: '2021-2022', title: 'Curso CSS - Victor Robles', text: 'Udemy', aos: 'fade-up' },
          { id: 7, ano: '2022', title: 'Formacion Vue', text: 'Udemy', aos: 'fade-up' },
          { id: 8, ano: '2022-2023', title: 'Formacion Flutter', text: 'Udemy/Youtube', aos: 'fade-up' },
          { id: 9, ano: '2023', title: 'Formación React', text: 'Youtube', aos: 'fade-up' },
      ]
  
      return {
        estudios
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
  section .trabajo-container {
    display: flex;
    width: 80%;
    height: 80px;
    margin: 0px;
    overflow: hidden;
  }
  
  .trabajo_title {
    display: flex;
    grid-row: auto;
    align-items: center;
    margin-top: 100px;
  }
  
  section .trabajo_title span {
    font-size: 26px;
    font-family: Overlock;
    margin-left: 20px;
  }
  
  .card {
    background: #02061a;
  }
  
  .card_year {
    width: 120px;
    background: #9d9ce3;
    border-radius: 5px;
    color: white;
    font-weight: 500;
    padding: 3px 15px 3px 15px;
  }
  
  .card-body {
    text-align: center;
  }
  
  .btn-proyecto {
    width: 120px;
    background: #9d9ce3;
    border-radius: 5px;
    color: white;
    font-weight: 500;
    padding: 3px 15px 3px 15px;
  }
  
  .hori-timeline .events .event-list {
      display: block;
      position: relative;
      text-align: center;
      padding-top: 70px;
      margin-right: 0;
  }
  .hori-timeline .events .event-list:before {
      content: "";
      position: absolute;
      height: 24px;
      border-right: 2px dashed #dee2e6;
      top: 20px;
  }
  .hori-timeline .events .event-list .event-date {
      position: absolute;
      top: 38px;
      left: 0;
      right: 0;
      width: 75px;
      margin: 0 auto;
      border-radius: 4px;
      padding: 2px 4px;
  }
  @media (min-width: 1140px) {
      .hori-timeline .events .event-list {
          display: inline-block;
          width: 24%;
          padding-top: 45px;
      }
      .hori-timeline .events .event-list .event-date {
          top: -12px;
      }
  }
  .bg-soft-primary {
      background-color: #9d9ce3 !important;
  }
  
  .list-inline-item {
    padding: 30px;
  } 
  
  </style>
  