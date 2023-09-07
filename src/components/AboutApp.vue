<template>
  <section class="about-app-store" id="us">
    <div class="container-fluid p-0">
      <div class="row no-gutters">
        <div class="col-lg-6">
          <div class="about-app section-padding bg-cover" :style="bgImg">
            <div class="section-title title-style-4 text-center">
              <h2 class="title">¿QUIENES SOMOS?</h2>
            </div>
            <div class="about-app-content text-center">
              <p class="mx-5">
                Somos una startup peruana que nace durante la pandemia buscando atender
                las necesidades de muchas personas con discapacidad temporal o permanente,
                haciendo uso de la tecnología digital y facilitando herramientas de
                gestión para los profesionales.
              </p>
              <br />
              <a href="https://fisioacasa.pe/appointment" class="read-more round-gradient"
                >AGENDA TU CITA</a
              >
            </div>
          </div>
        </div>
        <div class="col-lg-6">
          <CounterUp />
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
img {
  height: 3.5vh;
  margin-bottom: 0.75rem;
  margin-right: 0.1rem;
}

.title {
  font-size: 30px !important;
}

.fisio_link {
  color: white;
  text-decoration-color: #ed6c14;
  font-weight: bolder;
  font-size: 1.1rem;
}

p {
  color: white !important;
}
</style>
<script>
import CounterUp from "../components/CounterUp";
export default {
  components: {
    CounterUp,
  },
  data() {
    return {
      bgImg: {
        backgroundImage: `url(${require("../assets/img/bg/bgfi.png")})`,
      },
    };
  },
};
</script>
