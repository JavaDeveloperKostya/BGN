<script>
import Header from "./components/Header.vue"
import ContentAbout from "./components/ContentAbout.vue"
import ContentSkills from "./components/ContentSkills.vue"
import ContentProjects from "./components/ContentProjects.vue"
import ContentForm from "./components/ContentForm.vue"
import Footer from "./components/Footer.vue"
export default {
    data() {
        return {
        }
    },
    components: {
        Header,
        ContentAbout,
        ContentSkills,
        ContentProjects,
        ContentForm,
        Footer
    }
}
</script>

<template>
    <Header />
    <ContentAbout />
    <ContentSkills />
    <ContentProjects />
    <ContentForm />
    <Footer />
</template>

<style>
* {
    font-family:'Trebuchet MS';
    font-weight:bold;
    margin: 0px;
    padding: 0px;
    box-sizing: border-box;
    list-style-type: none;
    text-decoration: none;
    scroll-behavior: smooth;
}
</style>
