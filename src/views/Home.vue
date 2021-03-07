<template>
  <div id="home-container" class="d-flex flex-column flex-md-row">
    <div class="flex-same-width flex-column">
      <h1 class="text-h1 font-weight-bold primary-color">Olá !</h1>

      <p class="text-subtitle-1 white--text text-justify">
        Somos as psicólogas Ruth Braga (CRP 01-20774), Natália Ribeiro (CRP
        01-23593) e Nicole Xavier (CRP-01/23718), estamos disponibilizando vagas
        para atendimento social comunitário online.
      </p>

      <p class="text-subtitle-1 white--text text-justify">
        Decidimos criar este projeto com o intuito de proporcionar à comunidade
        os conhecimentos que nos foram adquiridos em nossos anos de formação e
        aprimoramento.
      </p>
    </div>

    <div class="flex-same-width">Teste</div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "Home",
});
</script>

<style lang="scss">
#home-container {
  padding: 50px;
  background-color: black;
}
</style>
