<template>
    <section class="service-area fix section-padding bg-cover pb-0 section pb-1" id="service" :style="bgImg">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="section-title title-style-5 text-center">
                        <h2 class="title">BENEFICIOS</h2>
                        <p class="paragraph">Conoce las ventajas de nuestra plataforma:</p>
                    </div>
                </div>
            </div>
            <div class="row service-item-inner">
                <!-- service single item start -->
                <div class="col-lg-4 col-md-6">
                    <div v-for="(service, services) in services" :key="services" class="service-item service-item__left">
                        <div class="service-icon">
                            <img :src="service.icon" alt="service icon">
                        </div>
                        <div class="service-content">
                            <h6>{{ service.title }}</h6>
                            <p>{{ service.desc }}</p>
                        </div>
                    </div>
                </div>
                <!-- service single item start -->

                <!-- service thumb start -->
                <div class="col-lg-4 order-3 order-lg-2">
                    <div class="service-middle-thumb">
                        <img src="../assets/img/home-medical/services.png" alt="service thumb" style="
                            width: 110%;
                            position: absolute;
                            bottom: 0%;
                        ">
                    </div>
                </div>
                <!-- service thumb  -->

                <!-- service single item start -->
                <div class="col-lg-4 col-md-6 order-2 order-lg-3">
                    <div v-for="(service2, services2) in services2" :key="services2"
                        class="service-item service-item__right">
                        <div class="service-icon">
                            <img :src="service2.icon" alt="service icon">
                        </div>
                        <div class="service-content">
                            <h6>{{ service2.title }}</h6>
                            <p>{{ service2.desc }} <br>
                                <span v-if="service2.down">{{ service2.down }}</span>
                            </p>
                        </div>
                    </div>
                </div>
                <!-- service single item start -->
            </div>
        </div>
    </section>
</template>

<style>
.service-content {
    text-align: center;
    color: #322d2deb !important;
}
</style>

<script>
export default {
    name: 'Benefits',
    data() {
        return {
            bgImg: {
                backgroundImage: `url(${require('../assets/img/home-medical/service-bg.jpg')})`
            },
            services: [
                {
                    title: "AHORRA TU TIEMPO",
                    desc: "Evita desplazarte y esperar ser atendido",
                    icon: require("../assets/img/icon/4.png")
                },
                {
                    title: "DISPONIBILIDAD",
                    desc: "Encuentra Fisioterapeutas donde estés y en el horario de tu preferencia",
                    icon: require("../assets/img/icon/calendarcheck.png")
                },
                {
                    title: "COMODIDAD Y PRIVACIDAD",
                    desc: "Serás atendido en el lugar que tú quieras",
                    icon: require("../assets/img/icon/smile.png")
                },
            ],
            services2: [
                {
                    title: "PAGOS SEGUROS",
                    desc: "A través de la pasarela de pagos de nuestra plataforma",
                    //down:"*La plataforma calcula el precio final*.", 
                    icon: require("../assets/img/icon/card.png")
                },
                {
                    title: "INFORMACION DE PROGRESO",
                    desc: "Gráficos intuitivos que muestran la evolución de tu recuperación",
                    icon: require("../assets/img/icon/stairs.png")
                },
                {
                    title: "SEGURIDAD Y CONFIANZA",
                    desc: "Revisamos antecedentes y validamos la habilidad profesional de los Fisioterapeutas",  
                    icon: require("../assets/img/icon/3.png")
                },
            ]
        }
    }
}
</script>

<style lang='scss'>
@import '../assets/scss/variables.scss';
@import '../assets/scss/components/service.scss';
</style>
