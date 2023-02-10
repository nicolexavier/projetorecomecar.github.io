<template>
	<div style="position: relative; height: 100%;">
		<div id="about-background">
			<div class="d-flex flex-column flex-md-row justify-center align-center container-spacing" style="height: 100%; background-color: rgba(0,0, 0, 0.75); background-attachment: scroll !important;">
				<div class="d-flex flex-column px-8 py-4 pr-md-16 pa-md-10">
					<h1 class="text-h1 font-weight-bold secondary-color">Olá!</h1>

					<p class="main-text white--text text-justify">
						Somos as psicólogas <strong>Natália Ribeiro</strong> (CRP 01/2359-3) e <strong>Ruth Braga</strong> (CRP
						01/2077-4) e estamos disponibilizando vagas para atendimento social online.
					</p>

					<p class="main-text white--text text-justify">
						Decidimos criar este projeto com o intuito de proporcionar à comunidade os conhecimentos que nos foram
						adquiridos em nossos anos de formação e aprimoramento.
					</p>

					<p class="main-text white--text text-justify">
						Além de nós, contamos também com a colaboração de outros psicólogos:

						<br />

						<span style="margin-left: 1.3rem">
							- Fernando Fernandes (CRP 01/2364-7)
						</span>

						<br />

						<span style="margin-left: 1.3rem">
							- Izabela Cristina Pereira Cordeiro (CRP 01/2256-8)
						</span>

						<br />

						<span style="margin-left: 1.3rem">
							- Karoline Oliveira (CRP 01/2416-1)
						</span>

					</p>
				</div>

				<img src="../assets/psicologo2-minified.jpg" />
			</div>
		</div>

		<div class="d-flex flex-column flex-md-row align-center justify-center container-spacing pt-10 pb-md-10">
			<div class="col-content-start">
				<h1 id="left-side-title" class="text-center font-weight-bold secondary-color">
					“Como a psicoterapia pode me ajudar?”
				</h1>
			</div>


			<div class="d-flex flex-column py-5 px-8 ml-md-10 col-content-end">
				<p class="main-text black--text font-weight-bold text-justify mt-3">
					A psicoterapia é um processo seu, que exigirá um trabalho colaborativo entre o psicólogo e você.
				</p>

				<p class="main-text black--text font-weight-bold text-justify">
					O psicólogo irá te auxiliar na busca por novos caminhos a serem trilhados, com o intuito de alcançar seus
					objetivos; utilizando de escuta sem julgamentos, empatia e acolhimento, além de técnicas comportamentais
					baseadas em evidências.
				</p>

				<p class="main-text black--text font-weight-bold text-justify">
					No nosso projeto, contamos também com psicólogos que possuem pós graduação em terapia de casal, sendo assim, o projeto também abarca casais que precisem de psicoterapia com este objetivo. 
				</p>

				<p class="main-text black--text font-weight-bold text-justify">
					<strong>Se seu objetivo for apenas psicoterapia individual, se inscreva através do formulário no fim da página.</strong>
				</p>

				<p class="main-text black--text font-weight-bold text-justify">
					Caso o atendimento seja para casal, inscreva-se através do formulário abaixo:
				</p>

				<v-btn class="mt-5 mb-14 mb-md-5 subscribe-btn" color="primary" style="font-weight: bold; color:white;" href="https://docs.google.com/forms/d/e/1FAIpQLSfFJJ3fQbypv95pxyihUSqZuPaCCWxHMARnz6bpOp0bcN1Vqw/viewform" target="_blank">INSCREVA-SE PARA TERAPIA DE CASAL</v-btn>
			</div>
		</div>

		<div class="d-flex flex-column flex-md-row align-center justify-center container-spacing pt-10 pb-md-16" style="background-color: #93a889;">
			<div class="col-content-start">
				<img src="../assets/atendimento-minified.jpg"/>
			</div>
			

			<div class="d-flex flex-column py-6 px-8 ml-md-10 col-content-end">
				<h1 class="text-h2 text-md-h1 font-weight-bold white--text">
					Participe!
				</h1>

				<p class="main-text white--text text-justify mt-3">
					Este projeto busca promover acessibilidade ao atendimento psicológico para a população. Este é um projeto
					autônomo, sem parceria com instituições, feito por psicólogas.
				</p>

				<p class="main-text white--text text-justify">
					As sessões de atendimento serão exclusivamente online, com duração entre 45 e 50 minutos, semanalmente, e
					serão agendadas de acordo com a disponibilidade de agenda das psicólogas.
				</p>

				<p class="main-text white--text text-justify">
					Para mais informações, se inscreva pelo formulário clicando no link abaixo:
				</p>

				<v-btn class="mt-5 mb-14 mb-md-5 subscribe-btn" color="primary" style="font-weight: bold; color:white;" href="https://docs.google.com/forms/d/1KVUyfst4wL4fvyX1bqX_lesBq6Sqa1OtkSjs4hIG-VE/edit?usp=sharing" target="_blank">INSCREVA-SE PARA PSICOTERAPIA INDIVIDUAL</v-btn>
			</div>
		</div>

		<div id="footer">
			© 2023 - Direitos reservados às sócias do Projeto Recomeçar.
		</div>
	</div>
</template>

<script lang="ts">
import Vue from 'vue';

export default Vue.extend({
	name: 'Home',
});
</script>

<style lang="scss">
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
	#about-background {
		background-image: url('../assets/monstera_2-minified.jpg') !important;
		background-position: center;
		background-repeat: no-repeat;
		background-size: cover;
	}

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

	#about-background {
		height: 100vh;
	}

	.subscribe-btn {
		font-size: 0.7rem!important;
	}

	.col-content-end {
		width: 100%;
	}
}

@media (min-width: 960px) {
	#about-background {
		background-image: url('../assets/monstera_2-minified.jpg') !important;
		background-position: center;
		background-repeat: no-repeat;
		background-size: cover;
		background-attachment: fixed;
	}
	
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

	.col-content-start {
		width: 40%;
	}

	.col-content-end {
		width: 60%;
	}

	#about-background {
		height: 95vh;
	}

	.subscribe-btn {
		font-size: 1rem;
	}
}

@media (max-width: 1400px) {
	#left-side-title {
		font-size: 4rem;
	}
}

@media (min-width: 1400px) {
	#left-side-title {
		font-size: 5rem;
	}
}

</style>
