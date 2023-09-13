<template>
  <section class="trabajo-container col-8 offset-2 pb-5" data-aos="fade-up"
     data-aos-anchor-placement="top-center">
    <div class="col-10 col-xxl-12 trabajo_title p-3 pb-5">
        <hr width="50" size="4" class="text-white" />
        <span class="text-white">Contacto</span>
    </div>

      <div class="row mb-5 pb-5">
        <div class="col-12 col-lg-6 mt-3">
          <img src="@/assets/contact.png" class="about_foto img-fluid" /> 
        </div>
        <div class="col-12 col-lg-5 offset-lg-1 mt-5 text-left">
          <!-- @submit.prevent="sendEmail" -->
          <form  class="text-left">
            <div class="mb-2">
              <label class="label">Nombre</label>
              <input
                class="form-control"
                type="text" 
                v-model="name"
                name="name"
                placeholder="Nombre" 
              >
            </div>
            <div class="mb-2">
              <label class="label">Email</label>
              <input 
                class="form-control"
                type="email" 
                v-model="email"
                name="email"
                placeholder="Email"
                >
            </div>
            <div class="mb-2">
              <label class="label">Mensaje</label>
              <textarea 
                class="form-control"
                name="message"
                v-model="message"
                cols="30" rows="3"
                autogrow
                placeholder="Mensaje">
              </textarea>
            </div>
            <div>
              <input class="button" type="submit" aria-label="Close" value="Enviar">
            </div>
          </form>
        </div>
        
        <div id="my-alert" class="alert alert-success alert-dismissible fade show" style="display: none;">
          <strong>Enviado!</strong> Tu mensaje ha sido enviado correctamente.
          <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
        </div>
        <div id="my-alert-error-campos" class="alert alert-danger alert-dismissible fade show" style="display: none;">
          <strong>Error!</strong> Tienes que llenar todos los campos.
          <button type="button" class="btn-close" data-bs-dismiss="alert-campos"></button>
        </div>
      </div>
    
  </section>
</template>

<script>
//import emailjs from 'emailjs-com';

export default {
  name: 'ContactComp',
  data() {
    return {
      name: '',
      email: '',
      message: ''
    }
  },
  /*methods: {
    sendEmail(e) {
      try {
        if (this.email !== '' && this.name !== '' && this.message !== '') {
          emailjs.sendForm('service_e7ztfhn', 'template_kl2vcmp', e.target, 'user_rGzDJ3jzggwpLvcqFZOgV', {
            name: this.name,
            email: this.email,
            message: this.meessage
          })
          console.log('Email enviado')
          this.showModal();
        } else this.showModal();

      } catch (error) {
          console.log({error})
      }
      // Reset form field
      this.name = ''
      this.email = ''
      this.message = ''
    },
    showModal () {
      if (this.email !== '' && this.name !== '' && this.message !== '') {
        document.getElementById("my-alert").style.display = "block";
        setInterval(() => { 
          document.getElementById("my-alert").style.display = "none";
        }, 3000);
      } else {
        document.getElementById("my-alert-error-campos").style.display = "block";
        setInterval(() => { 
          document.getElementById("my-alert-error-campos").style.display = "none";
        }, 3000);
      }
    }
  }*/
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


.label {
  color: white;
  font-family: Overlock;
  padding-top: 5px;
  padding-bottom: 5px;
  text-align: left;
  display: flex;
}

.button{
  position: relative;
  background-color: #9d9ce3;
  border: 0px;
  border-radius: 4em;
  font-size: 16px;
  color: white;
  padding: 0.8em 1.8em;
  cursor: pointer;
  display: flex;
  justify-self: start;
  justify-content: center;
  text-align: left;
  text-decoration: none;
  cursor: pointer;
  width: 35%;
  transition-duration: 0.4s;
  -webkit-transition-duration: 0.4s; /* Safari */
}

.button:hover {
  transition-duration: 0.1s;
  background-color: #6867bb;
}

.button:after {
  content: "";
  display: block;
  position: absolute;
  border-radius: 4em;
  left: 0;
  top:0;
  width: 100%;
  height: 100%;
  opacity: 0;
  transition: all 0.5s;
  box-shadow: 0 0 10px 40px white;
}

.button:active:after {
  box-shadow: 0 0 0 0 white;
  position: absolute;
  border-radius: 4em;
  left: 0;
  top:0;
  opacity: 1;
  transition: 0s;
}

.button:active {
  top: 1px;
}



</style>
