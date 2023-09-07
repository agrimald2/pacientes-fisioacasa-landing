<template>
    <div class="main-container">

        <!-- Navbar section -->
        <Navbar NavbarStyle="NavbarStyle" />

        <!-- slider section -->
        <HeroBanner />

        <!-- Nosotros --> 
        <AboutApp/>
        
        <!-- Beneficios --> 
        <Benefits/>

        <Find/>
        
        <How/>

<!--
        <Requirements/>
-->

    

        <!--
            
        -->
        <Faq/>

    <div class="elfsight-app-29c2eb41-262a-4b0e-b63e-8f3ea4b655db"></div>    

        
        <Footer/>
        
        <!-- about section 
        <About AboutStyle="about-style-2" />
        -->
    </div>
</template>

<script>
    import Navbar from '../components/Navbar'
    import HeroBanner from '../components/HeroBanner'
    import AboutApp from '../components/AboutApp'
    import Benefits from '../components/Benefits'
    import Find from '../components/Find'
    import How from '../components/How'
    import Requirements from '../components/Requirements'
    import Faq from '../components/Faq'
    import Footer from '../components/Footer'
    //import About from '../components/About'
    

    export default {
        name: 'app',
        components: {
            Navbar,
            HeroBanner,
            AboutApp,
            Benefits,
            Find,
            How,
            Faq,
            Requirements,
        //    About,
            Footer,
        }
    }
</script>

