<template>
    <section class="department-area section-padding bg-cover section" id="department" :style="bgImg">
        <div class="container">
            <div class="row">
                <div class="col-lg-6">
                    <div class="section-title title-style-5 section-title__left">
                        <h2 class="title">PREGUNTAS FRECUENTES</h2>
                        <p class="paragraph">A continuación, te detallamos una lista de las preguntas que más nos hacen
                        </p>
                    </div>
                    <div class="department-faq">
                        <b-card no-body class="mb-1">
                            <b-card-header header-tag="header">
                                <b-button block href="#" v-b-toggle.accordion-1 variant="info"><span>0.1</span> ¿Debo elegir al mismo fisioterapeuta y ubicación para un tratamiento?</b-button>
                            </b-card-header>
                            <b-collapse id="accordion-1" visible accordion="my-accordion">
                                <b-card-body>
                                        <!--<img src="../assets/img/home-medical/departments.jpg" alt="doctor thumb"
                                            class="dep-thumb"> -->
                                    <b-card-text>

                                        <p>
                                            La plataforma permite agregar múltiples ubicaciones para que los pacientes puedan continuar sus tratamientos en el lugar de su mejor conveniencia.

                                        </p>
                                        <!--<a class="learn-more" href="#">Learn More</a>-->
                                    </b-card-text>
                                </b-card-body>
                            </b-collapse>
                        </b-card>

                        <b-card no-body class="mb-1">
                            <b-card-header header-tag="header">
                                <b-button block href="#" v-b-toggle.accordion-2 variant="info"><span>0.2</span> ¿Cómo puedo conocer el progreso de mi tratamiento?</b-button>
                            </b-card-header>
                            <b-collapse id="accordion-2" accordion="my-accordion">
                                <b-card-body>
                                    <!--<img src="../assets/img/home-medical/departments.jpg" alt="doctor thumb"
                                        class="dep-thumb"> -->
                                    <b-card-text>

                                        <p>
 La evolución de la recuperación de cada paciente puede ser visualizada a través de gráficos e indicadores de bienestar en tiempo real. Cada paciente es libre de escoger al o los profesionales que necesite para gestionar su tratamiento. 

                                        </p>
                                    </b-card-text>
                                </b-card-body>
                            </b-collapse>
                        </b-card>

                        <b-card no-body class="mb-1">
                            <b-card-header header-tag="header">
                                <b-button block href="#" v-b-toggle.accordion-3 variant="info"><span>0.3</span> ¿CÓMO SE
                                    REALIZAN LOS PAGOS?</b-button>
                            </b-card-header>
                            <b-collapse id="accordion-3" accordion="my-accordion">
                                <b-card-body>
                                    <!--<img src="../assets/img/home-medical/departments.jpg" alt="doctor thumb"
                                        class="dep-thumb"> -->
                                    <b-card-text>

                                        <p>
                                            Se realizan a través de una pasarela de pagos integrada que de forma
                                            automática le permitirá usar su cuenta bancaria afiliada para tal fin. Los
                                            pagos pueden ser liquidados quincenal o mensualmente. El dinero recaudado de
                                            los servicios es asignado de forma inmediata al finalizar el servicio.
                                        </p>
                                    </b-card-text>
                                </b-card-body>
                            </b-collapse>
                        </b-card>

                        <b-card no-body class="mb-1">
                            <b-card-header header-tag="header">
                                <b-button block href="#" v-b-toggle.accordion-4 variant="info"><span>0.4</span> ¿CÓMO
                                    VISUALIZO LA EVOLUCIÓN DE MIS PACIENTES?</b-button>
                            </b-card-header>
                            <b-collapse id="accordion-4" accordion="my-accordion">
                                <b-card-body>
                                    <!--<img src="../assets/img/home-medical/departments.jpg" alt="doctor thumb"
                                        class="dep-thumb"> -->
                                    <b-card-text>

                                        <p>
                                            La plataforma cuenta con un módulo de gestión de tratamientos e historias
                                            clínicas donde los profesionales podrán visualizar de manera gráfica y con
                                            indicadores de bienestar la evolución y progreso de cada uno de sus
                                            pacientes.
                                        </p>
                                    </b-card-text>
                                </b-card-body>
                            </b-collapse>
                        </b-card>

                        <b-card no-body class="mb-1">
                            <b-card-header header-tag="header">
                                <b-button block href="#" v-b-toggle.accordion-5 variant="info"><span>0.5</span> ¿Cómo
                                    funciona el sistema de tarifas?</b-button>
                            </b-card-header>
                            <b-collapse id="accordion-5" accordion="my-accordion">
                                <b-card-body>
                                    <b-card-text>
                                        <p>
                                            Los profesionales ingresan su monto neto a recibir y la plataforma calcula
                                            los costos adicionales (margen comercial, transporte, impuestos y EPPs) para
                                            mostrar el precio final que el cliente tendrá que pagar.
                                        </p>
                                    </b-card-text>
                                </b-card-body>
                            </b-collapse>
                        </b-card>

                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
.paragraph {
    color: white !important;
}
</style>
<script>
export default {
    name: 'Department',
    data() {
        return {
            bgImg: {
                backgroundImage: `url(${require('../assets/img/fisio-bg2.png')})`
            }
        }
    }
}
</script>
