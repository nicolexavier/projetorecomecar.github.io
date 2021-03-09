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
            <h1 class="text-h1 font-weight-bold secondary-color">Olá!</h1>

            <p class="text-subtitle-1 white--text text-justify">
              Somos as psicólogas <strong>Natália Ribeiro</strong> (CRP
              01-23593), <strong>Nicole Xavier</strong> (CRP 01-23718) e
              <strong>Ruth Braga</strong> (CRP 01-20774), estamos
              disponibilizando vagas para atendimento social online.
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
        <h1 class="text-h2 text-md-h1 font-weight-bold secondary-color">
          Participe!
        </h1>

        <p class="text-subtitle-1 black--text text-justify mt-3">
          Este projeto busca promover a acessibilidade ao atendimento
          psicológico para a população. Este é um projeto autônomo, sem parceria
          com instituições, feito por psicólogas.
        </p>

        <p class="text-subtitle-1 black--text text-justify">
          As sessões de atendimento serão exclusivamente online, com duração
          entre 45 e 50 minutos semanalmente, e serão disponibilizadas de acordo
          com a disponibilidade de agenda das psicólogas.
        </p>

        <p class="text-subtitle-1 black--text text-justify">
          Para mais informações, se inscreva pelo formulário clicando no link
          abaixo:
        </p>

        <v-btn
          class="mt-5 mb-8 mb-md-5"
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
  position: relative;
  height: 5vh;
  width: 100vw;

  background-color: black;
}

#subscribe-btn {
  color: white;
  font-weight: bolder;
  background-color: #93a889;
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
    margin-top: 25vh;
  }

  #footer {
    margin-top: 20vh;
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
