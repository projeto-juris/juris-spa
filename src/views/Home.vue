<template>
  <div>
    <v-app-bar id="appBar" app color="transparent" style="position: absolute !important;" flat>
      <a>
        <v-img id="img" src="../assets/logoJuris.svg" />
      </a>
      <v-spacer></v-spacer>
      <v-btn text small color="white">Sobre</v-btn>
      <v-btn text small color="white" @click="scrollIntoView('about')">Como usar</v-btn>
      <v-btn text small @click="scrollIntoView('services')" color="white">Serviços</v-btn>
      <v-btn text small @click="scrollIntoView('FAQ')" color="white">FAQ</v-btn>
      <v-btn text small color="white" @click="scrollIntoView('footer')">Contato</v-btn>
      <v-btn large color="primary">Login</v-btn>
    </v-app-bar>
    <v-main>
      <v-lazy>
        <v-container class="vContainer">
          <v-card id="vCard" color="transparent" outlined width="35%">
            <p id="cardText">
              Torne o seu fluxo
              <br />de atendimento aos seus clientes
              <br />mais simples
            </p>
            <v-card-actions>
              <v-btn color="primary" large rounded>Contrate agora</v-btn>
            </v-card-actions>
          </v-card>
        </v-container>
      </v-lazy>
      <v-lazy style="margin-top: 64px;">
        <About id="about" />
      </v-lazy>
      <v-lazy>
        <Services id="services" />
      </v-lazy>
      <v-lazy>
        <FAQ id="FAQ" />
      </v-lazy>
    </v-main>
    <v-lazy>
      <Footer id="footer" />
    </v-lazy>
  </div>
</template>

<script>
import About from "../components/About/About.vue"
import Services from "../components/servicesComponent/Services.vue"
import FAQ from "../components/FAQ/Faq.vue"
import Footer from "../views/footer.vue"
export default {
  name: "Home",
  components: {
    About,
    Services,
    FAQ,
    Footer,
  },
  methods: {
    scrollIntoView(el) {
      var elmnt = document.getElementById(el)
      elmnt.scrollIntoView({ behavior: "smooth" })
    },
  },
}
</script>
<style>
#cardText {
  font-size: 3em;
  font-weight: normal;
  color: white;
  line-height: 1;
}
#vCard {
  display: block;
  margin-left: 20%;
}
.vContainer {
  height: 100vh;
}
#img {
  max-width: 90px;
}
#app > div > main {
  padding: 0 !important;
}
</style>
