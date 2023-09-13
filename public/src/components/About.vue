<template>
  <section class="about-container col-8 offset-2 pb-5">
   <div class="row cont justify-content-center p-0 m-0">
     <div class="col-10 col-xxl-12 about_title p-3 pb-5">
       <hr width="50" size="4" class="text-white" />
       <span class="text-white">Sobre mi</span>
     </div>

     <div class="col-12 col-sm-8 col-lg-4" data-aos="fade-right">
         <div class="w-250 wrapper">
             <svg viewBox="0 0 500 500" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="100%" id="blobSvg">
                 <defs>
                     <clipPath id="shape">
                       <path id="blob" d="M454.5,289Q438,328,425.5,370.5Q413,413,373,431.5Q333,450,291.5,460Q250,470,209.5,457.5Q169,445,126,431Q83,417,51.5,381Q20,345,27,297.5Q34,250,33.5,205Q33,160,64.5,128Q96,96,126,59.5Q156,23,203,23.5Q250,24,298,21.5Q346,19,380,52.5Q414,86,441.5,122.5Q469,159,470,204.5Q471,250,454.5,289Z" fill="#d1d8e0"></path>
                     </clipPath>
                 </defs>
                 <image id="slide" x="0" y="0" width="100%" height="100%" clip-path="url(#shape)" xlink:href="https://res.cloudinary.com/dtwzcfryn/image/upload/v1644482948/foto2_perfil_vg7cs3.png" preserveAspectRatio="none"></image>
             </svg>
         </div>
       <!-- <img src="@/assets/foto.png" class="about_foto img-fluid" /> -->
     </div>
     <div class="col-12 col-sm-8 col-lg-5 offset-lg-2 col-xxl-6 offset-xxl-2" data-aos="fade-left">
       <div class="row">
         <div class="about_box_anos m-1 col-lg-4 col-xxl-2">
           <img src="@/assets/velas.png" height="30" />
           <p class="about_box_anos_title text-center text-white">AÑOS</p>
           <p class="about_box_email_info text-center text-white">30</p>
         </div>
         <div class="about_box_email m-1 col-lg-7 col-xxl-4">
           <img src="@/assets/email_icon.png" height="30" />
           <p class="about_box_email_title text-center text-white">EMAIL</p>
           <p class="about_box_email_info text-center text-white">dfont93@gmail.com</p>
         </div>
         <!-- <div class="row col-12 col-lg-4 mt-lg-2 col-xxl-2 text-right">
           <div class="column">
           <img src="@/assets/instagram.png" class="mt-3 float-right" height="30" />
           <img src="@/assets/instagram.png" class="mt-3 float-right" height="30" />
           <img src="@/assets/instagram.png" class="mt-3 float-right" height="30" />
           </div>
         </div> -->
       </div>

       <div class="row pt-3">
         <p class="about_descripcion col-10 mt-4 text-white" >
           Desarrollador y diseñador Web que le gusta la simplicidad pero con un toque elegante y colorido. Con ganas de entrar en un proyecto aprender y crecer como programador. La fotografia de paisaje y el padel son mis hobbies fuera de la programación.
         </p>
       </div>
       <!-- <div class="row col-8 col-xl-4 pt-3">
         <button type="button" @click="download()" class="p-2 mt-4 ml-2 text-left btn btn-contact">DESCARGAR CV</button>
       </div>  -->

     </div>
   </div>
   
 </section>  
</template>


<script>
export default {
name: 'AboutComp'
}
</script>

<style lang="scss" scoped>

/****************************
         ABOUT
*****************************/


.cont {
  display: flex;
  width: 100%;
  
  background-color: #02061a;
}

.info {
  display: flex;
}

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

.about_descripcion {
  text-align: left;
}

.about_foto {
  background: #ae59e1;
  border-radius: 25px;
  transform: rotate(0deg);
  border: 4px solid #d986ee;
  min-width: 225px;
  min-height: 225px;
}

.about_box_anos, .about_box_email, .about_box_telefono {
height: auto;
left: 525px;
top: 541px;
background: #151C26;
border-radius: 15px;
}

.about_box_anos img, .about_box_email img, .about_box_telefono img{
margin-top: 7px;
}

.about_box_anos_title, .about_box_email_title, .about_box_telefono_title {
  margin-top: 18px;
  margin-bottom: 0px;
  font-size: 14px;
  font-weight: 600;
}

.about_box_anos_info, .about_box_email_info, .about_box_telefono_info {
  margin-top: 12px;
  font-size: 14px;
  font-weight: 500;
}

.btn-contact {
  background: #ae59e1;
  border-radius: 15px;
  color: white;
  font-family: Overlock;
  font-size: 20x;
}


</style>