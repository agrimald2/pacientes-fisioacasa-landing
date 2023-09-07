<template>
    <section class="testimonial-area-four section-padding section" :class="testimonialStyle" id="requirements">
        <div class="testimonial-top">
            <div class="container">
                <div class="row">
                    <div class="col-12">
                        <div class="section-title title-style-4 text-center">
                            <h2 class="title">Requisitos Necesarios</h2>
                            <p style="color: white;">Es importante contar con todo lo que se menciona abajo para ser parte de nosotros </p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="testimonial-bottom">
            <div class="container">
                <div class="row">
                    <div class="col-12">
                        <carousel class="testimonial-active-four owl-dot-style"
                            :items = "3"
                            :nav = "false"
                            :dots = "false"
                            :smartSpeed = "1000"
                            :responsive="{0:{items:1},768:{items:2},1200:{items:3}}"
                        >
                            <div v-for="(client, clients) in clients" :key="clients" class="testimonial-item">
                                <div class="testimonial-thumb" style="border-radius:0%">
                                    <img :src="client.clientThumb" alt="client thumb">
                                </div>
                                <div class="testimonial-content">
                                    <h6 class="client">{{ client.name }}  <span>{{ client.designation }}</span></h6>
                                    <!--<p>{{ client.desc }}</p>-->
                                </div>
                            </div>
                        </carousel>
                    </div>
                </div>
                <div class="row register_container">
                    <a href="https://fisioacasa.pe/appointment" class="read-more round-gradient">Regístrate</a>
                </div>
            </div>
        </div>

        <Instagram/>

    </section>
</template>
<style scoped>
.register_container{
    padding: 2rem;
    display: flex;
    justify-content: center;
}
.read-more{
        background-color: #ED6C14;
    }
    .client{
        font-size: 1.4rem;
        font-weight: 200;
    }
</style>
<script>
import carousel from 'vue-owl-carousel'
import Instagram from '../components/Instagram'
export default {
    name: 'TestimonialFour',
    components: { 
        carousel,
        Instagram 
    },
    props: ["testimonialStyle"],
    data (){
        return {
            clients: [
                {
                    clientThumb: require("../assets/img/testimonial/r1.png"), 
                    name: "Ser un Fisioterapeuta Colegiado", 
                    designation: "", 
                    desc: "Claritas est etiam processus dynamicus, qui sequitur mutationem consuetudium lectorum. Mirum est notare quam littera gothica, quam nunc putamus parum claram..."
                },
                {
                    clientThumb: require("../assets/img/testimonial/r2.png"), 
                    name: "Tener Habilidad Profesional vigente", 
                    designation: "", 
                    desc: "Claritas est etiam processus dynamicus, qui sequitur mutationem consuetudium lectorum. Mirum est notare quam littera gothica, quam nunc putamus parum claram..."
                },
                {
                    clientThumb: require("../assets/img/testimonial/r3.png"), 
                    name: "Certificado de Antecedentes Penales y Policiales", 
                    designation: "", 
                    desc: "Claritas est etiam processus dynamicus, qui sequitur mutationem consuetudium lectorum. Mirum est notare quam littera gothica, quam nunc putamus parum claram..."
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
