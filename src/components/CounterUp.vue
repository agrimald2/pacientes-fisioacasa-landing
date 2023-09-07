<template>
    <!--@TODO CHANGE ICONS, BOLSA DE DINERO, CALENDARIO, CABIFY, -->
    <div  class="fun-fact-area">
        <!-- single counterup start -->
        <div class="single-funfact">
            <div class="funfact-inner">
                <div class="funfact-icon">
                    <img src="../assets/img/icon/patients.png" alt="">
                </div>
                <span> RED DE FISIOTERAPEUTAS</span>
                <p>A NIVEL NACIONAL</p>
            </div>
        </div>
        <!-- single counterup end -->

        <!-- single counterup start -->
        <div class="single-funfact">
            <div class="funfact-inner">
                <div class="funfact-icon">
                    <img src="../assets/img/icon/calendar.png" alt="">
                </div>
                <span>
                    GESTIÓN DE CITAS
                </span>
                <p>PLATAFORMA WEB</p>
            </div>
        </div>
        <!-- single counterup end -->

        <!-- single counterup start -->
        <div class="single-funfact">
            <div class="funfact-inner">
                <div class="funfact-icon">
                    <img src="../assets/img/icon/3.png" alt="">
                </div>
                <span>SEGURIDAD</span>
                <p>PERSONAL VALIDADO</p>
            </div>
        </div>
        <!-- single counterup end -->

        <!-- single counterup start -->
        <div class="single-funfact">
            <div class="funfact-inner">
                <div class="funfact-icon">
                    <img src="../assets/img/icon/hands.png" alt="">
                </div>
                <span>CONFIANZA</span>
                <p>FISIOTERAPEUTAS COLEGIADOS</p>
            </div>
        </div>
        <!-- single counterup end -->
    </div>
</template>
<style scoped>
    span{
        font-size: 1.5rem!important;
    }
    .funfact-inner p{
        font-size: 1rem;
    }
</style>
<script>
    //import ICountUp from 'vue-countup-v2';
    export default {
        name: 'demo',
        components: {
            //ICountUp
        },
        data() {
            return {
                delay: 300
            };
        }
    };
</script>

<style lang='scss'>
    @import '../assets/scss/variables.scss';
    @import '../assets/scss/components/counterup.scss';
</style>
