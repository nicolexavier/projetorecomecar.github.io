<template>
  <div class="d-flex flex-column">
    <div id="about-background">
      <div
        class="d-flex align-md-center justify-center mt-10 mt-md-0 h-100"
        style="background-color: rgba(0,0, 0, 0.75); background-attachment: scroll !important;"
      >
        <div
          class="d-flex flex-column flex-md-row align-center container-spacing"
        >
          <div class="d-flex flex-column pa-10 pr-md-16">
            <h1 class="text-h1 font-weight-bold primary-color">Olá !</h1>

            <p class="text-subtitle-1 white--text text-justify">
              Somos as psicólogas <strong>Natália Ribeiro</strong> (CRP
              01-23593), <strong>Nicole Xavier</strong> (CRP 01-23718) e
              <strong>Ruth Braga</strong> (CRP 01-20774), estamos
              disponibilizando vagas para atendimento social comunitário online.
            </p>

            <p class="text-subtitle-1 white--text text-justify">
              Decidimos criar este projeto com o intuito de proporcionar à
              comunidade os conhecimentos que nos foram adquiridos em nossos
              anos de formação e aprimoramento.
            </p>
          </div>

          <img src="../assets/psicologo.jpg" />
        </div>
      </div>
    </div>

    <div
      class="d-flex flex-column flex-md-row align-center justify-center container-spacing"
      style="height: 60vh;"
      id="second-section"
    >
      <img src="../assets/atendimento.jpg" />

      <div class="d-flex flex-column pa-10">
        <h1 class="text-h2 text-md-h1 font-weight-bold primary-color">
          Participe !
        </h1>

        <p class="text-subtitle-1 black--text text-justify mt-3">
          Este projeto busca promover a acessibilidade ao atendimento
          psicológico a todos necessitados e interessados ao mesmo !
        </p>

        <p class="text-subtitle-1 black--text text-justify">
          As sessões de atendimento serão exclusivamente ONLINE e estarão
          disponíveis à preço social. Para mais informações, visualize o
          formulário clicando no botão abaixo ou envie um email para
          <strong>projetorecomecar@gmail.com</strong>."
        </p>

        <v-btn
          class="mt-5"
          id="subscribe-btn"
          href="https://docs.google.com/forms/d/1KVUyfst4wL4fvyX1bqX_lesBq6Sqa1OtkSjs4hIG-VE/edit?usp=sharing"
          target="_blank"
          >Increva-se AQUI !</v-btn
        >
      </div>
    </div>

    <div
      id="footer"
      class="d-flex justify-center align-center text-md-body-2 grey--text"
    >
      © 2021 - Direitos reservados às sócias do Projeto Recomeçar.
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";

export default Vue.extend({
  name: "Home",
});
</script>

<style lang="scss">
#about-background {
  background-image: url("../assets/monstera.png") !important;
  background-size: cover;
  background-attachment: fixed;
  background-repeat: no-repeat;
}

#footer {
  height: 5vh;
  width: 100vw;

  background-color: black;
}

#subscribe-btn {
  color: white;
  font-weight: bolder;
  background-color: #1cce1cd7;
}

@media (max-width: 960px) {
  img {
    width: 30vh;
    height: 30vh;
    border-radius: 250px;
    object-fit: cover;
  }

  .container-spacing {
    padding-left: 0;
    padding-right: 0;
  }

  #second-section {
    margin-top: 20vh;
  }

  #footer {
    margin-top: 18vh;
    font-size: 10px;
  }
}

@media (min-width: 960px) {
  img {
    width: 50vh;
    height: 50vh;
    border-radius: 250px;
    object-fit: contain;
  }

  .container-spacing {
    padding-left: 15vw;
    padding-right: 15vw;
  }
}
</style>
