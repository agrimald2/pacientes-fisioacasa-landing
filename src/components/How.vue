<template>
    <section class="testimonial-area pt-100 fix section" id="review" :style="bgImg">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div class="section-title text-center">
                        <div class="title-icon"></div>
                        <h2 class="title text-white">PASOS PARA AGENDAR TU CITA</h2>
                        <p style="color: black;">
                           En menos de <strong style="text-decoration: underline;"> 30 segundos</strong>
                        </p>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-12">
                    <carousel class="testimonial-active owl-dot-style"
                        :items="1"
                        :nav="true"
                        :smartSpeed="1000"
                        :navText="['<','>']"
                    >
                        <!-- testimonial item start -->
                        <div v-for="(client, clients) in clients" :key="clients" class="testimonial-item">
                            <div class="testimonial-thumb">
                                <img :src="client.clientThumb" alt="client thumb">
                            </div>
                            <div class="testimonial-content">
                                <h6 class="client"><span style="font-family: fantasy">{{client.admirationS}}</span> {{ client.name }} <span style="font-family: fantasy">{{client.admirationE}}</span> <br> <span>{{ client.designation }}</span></h6>
                                <p class="desc">{{ client.desc }}</p>
                            </div>
                        </div>
                        <!-- testimonial item end -->
                    </carousel>
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
    .title{
        color: #ED6C14!important;
    }
    .client{
        color: black;
        font-size: 1.3rem;
    }
    .desc{
        color: black;
        font-size: 1.1rem;
    }
</style>
<script>
import carousel from 'vue-owl-carousel'
export default {
    name: 'Testimonial',
    components: { 
        carousel 
    },
    data (){
        return {
            bgImg: {
                backgroundImage: `url(${require('../assets/img/blob-bg.png')})`
            },
            clients: [
                {
                    clientThumb: require("../assets/img/testimonial/1.png"), 
                    name: "INGRESA TU DNI", 
                    designation: "Completa tus datos personales", 
                    desc: ""
                },
                {
                    clientThumb: require("../assets/img/testimonial/2.png"), 
                    name: "SELECCIONA TU UBICACIÓN", 
                    designation: "", 
                    desc: ""
                },
                {
                    clientThumb: require("../assets/img/testimonial/3.png"), 
                    name: "ELIGE TU FISIOTERAPEUTA", 
                    designation: "Filtra por Especialidad, Ubicación, Calificaciones y Precios", 
                    desc: "Elige el que más te convenga"
                },
                {
                    clientThumb: require("../assets/img/testimonial/4.png"), 
                    admirationS: "¡",
                    admirationE: "!",
                    name: "Y LISTO", 
                    designation: "CITA AGENDADA", 
                    desc: "Recibe tu confirmación al Whatsapp y Correo electrónico"
                },
            ]
        }
    }
}
</script>

<style lang='scss'>
    @import '../assets/scss/variables.scss';
    @import '../assets/scss/components/testimonial.scss';
</style>
