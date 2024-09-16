<script>
// AppHeader, AppMain, AppFooter
// 1 - importo il componente dai component
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";

export default {
  data() {
    return {
      count: 0 
    }
  },
  components:{
    // 2 lo importo nella lista dei componenti del mio componente
    AppHeader,
    AppMain
  },
  methods: {},
  computed: {},
  mounted(){},
}
</script>

<template>
<!-- 3 - inserisco il mio componente dove voglio che sia visibile come self-closing tag -->
  <AppHeader />
  <AppMain />
</template>

<style lang="scss">
/*  inserisci qui dentro stile generico */
@use "./styles/partials/variables" as *;
@use "./styles/partials/mixins" as *;
@use "./styles/general.scss" as *;


body{
  @include reset;
}

ul{
  @include flex(row, space-between, center)
}

</style>
