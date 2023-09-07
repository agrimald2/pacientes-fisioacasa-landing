<template>
  <section class="slider-section hero-style-2 section" id="home" :style="bgImg">
    <div class="hero-slider-item">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-lg-6 col-md-6 order-2 order-md-1">
            <div class="slider-content slider-content__style-2">
              <p class="slider-desc">
                <span style="font-weight: bold"> </span>Somos una plataforma digital que
                conecta a pacientes con profesionales colegiados de Terapia Física.
              </p>
              <br />
              <h2 class="slider-title">
                <span style="font-family: 'Rubik'">¿</span>Necesitas un
                fisioterapeuta<span style="font-family: 'Rubik'">?</span>
              </h2>
              <div class="slider-btn">
                <a
                  href="https://fisioacasa.pe/appointment"
                  class="read-more active round-gradient"
                  style="background-color: #ed6c14"
                >
                  AGENDA TU CITA
                </a>
                <img class="sm:ml-2" src="../assets/img/logoCTMP.png" height="100px" width="auto">
              </div>
            </div>
          </div>
          <div class="col-lg-6 col-md-6 order-1 order-md-2">
            <div class="slider-banner-thumb slide-animate center">
              <img
                class="mt-5 md:mt-1"
                src="../assets/img/slider/appointment_confirmed.png"
                alt="slider thumb"
              />
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
<style scoped>
.slider-title {
  text-transform: uppercase;
}

.slider-desc {
  font-size: 1.2rem;
}

.slide-animate img {
  max-width: 70%;
}
@media (max-width: 576px) {
  .slide-animate img {
    max-width: 55%;
  }
}
</style>
<script>
export default {
  name: "HeroBanner",
  data() {
    return {
      bgImg: {
        backgroundImage: `url(${require("../assets/img/bg-home.png")})`,
      },
    };
  },
};
</script>
