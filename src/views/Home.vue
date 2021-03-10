<template>
  <div style="position: relative; height: 100%;">
    <div style="height: 88vh;" id="about-background">
      <div
        class="d-flex flex-column flex-md-row justify-center align-center container-spacing"
        style="height: 100%; background-color: rgba(0,0, 0, 0.75); background-attachment: scroll !important;"
      >
        <div class="d-flex flex-column px-11 py-4 pr-md-16 pa-md-10">
          <h1 class="text-h1 font-weight-bold secondary-color">Olá!</h1>

          <p class="main-text white--text text-justify">
            Somos as psicólogas <strong>Natália Ribeiro</strong> (CRP 01-23593),
            <strong>Nicole Xavier</strong> (CRP 01-23718) e
            <strong>Ruth Braga</strong> (CRP 01-20774), estamos disponibilizando
            vagas para atendimento social online.
          </p>

          <p class="main-text white--text text-justify">
            Decidimos criar este projeto com o intuito de proporcionar à
            comunidade os conhecimentos que nos foram adquiridos em nossos anos
            de formação e aprimoramento.
          </p>
        </div>

        <img src="../assets/psicologo.jpg" />
      </div>
    </div>

    <div
      class="d-flex flex-column flex-md-row align-center justify-center container-spacing pt-10 pb-md-10"
    >
      <h1
        class="text-h2 text-md-h1 text-center font-weight-bold secondary-color"
      >
        “Como a psicoterapia pode me ajudar?”
      </h1>

      <div class="d-flex flex-column py-5 px-11">
        <p class="main-text black--text font-weight-bold text-justify mt-3">
          A psicoterapia é um processo seu, que exigirá um trabalho colaborativo
          entre o psicólogo e você.
        </p>

        <p class="main-text black--text font-weight-bold text-justify">
          O psicólogo irá te auxiliar na busca por caminhos que façam sentido
          para você, com intuito de alcançar seus objetivos, utilizando de
          escuta sem julgamentos, empatia e acolhimento.
        </p>
      </div>
    </div>

    <div
      class="d-flex flex-column flex-md-row align-center justify-center container-spacing pt-10 pb-md-16"
      style="background-color: #93a889;"
    >
      <img src="../assets/atendimento.jpg" />

      <div class="d-flex flex-column py-6 px-11 ml-md-10">
        <h1 class="text-h2 text-md-h1 font-weight-bold white--text">
          Participe!
        </h1>

        <p class="main-text white--text text-justify mt-3">
          Este projeto busca promover acessibilidade ao atendimento psicológico
          para a população. Este é um projeto autônomo, sem parceria com
          instituições, feito por psicólogas.
        </p>

        <p class="main-text white--text text-justify">
          As sessões de atendimento serão exclusivamente online, com duração
          entre 45 e 50 minutos, semanalmente, e serão disponibilizadas de
          acordo com a disponibilidade de agenda das psicólogas.
        </p>

        <p class="main-text white--text text-justify">
          Para mais informações, se inscreva pelo formulário clicando no link
          abaixo:
        </p>

        <v-btn
          class="mt-5 mb-14 mb-md-5"
          id="subscribe-btn"
          color="primary"
          href="https://docs.google.com/forms/d/1KVUyfst4wL4fvyX1bqX_lesBq6Sqa1OtkSjs4hIG-VE/edit?usp=sharing"
          target="_blank"
          >Increva-se</v-btn
        >
      </div>
    </div>

    <div id="footer">
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
}

#subscribe-btn {
  color: white;
  font-weight: bolder;
}

#footer {
  color: grey;
  font-size: 0.8rem;
  padding: 10px;
  background-color: black;
  text-align: center;
  position: absolute;
  bottom: 0;
  width: 100%;
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
}

@media (min-width: 960px) {
  img {
    width: 50vh;
    height: 50vh;
    border-radius: 250px;
    object-fit: contain;
  }

  .container-spacing {
    padding-left: 12vw;
    padding-right: 12vw;
  }
}
</style>
