<script>
import HeaderNavbar from "./HeaderNavbar.vue";

export default {
    data() {
        return {
            // chiave : valore 

        }
    },
    components:{
        HeaderNavbar
    }
}
</script>

<template>
    <!-- sintassi vue -> chiave  => valore -->
     <!-- definire l'header della nostra applicazione -->
      <!-- istanziare il componente che contiene la navbar -->
    <header>
        <h1>
            Header
        </h1>
        <HeaderNavbar />
    </header>
</template>

<style lang="scss" scoped>
    @use "../styles/partials/variables" as *;

    h1{
        color: $text_accent_color;
    }

    

</style>