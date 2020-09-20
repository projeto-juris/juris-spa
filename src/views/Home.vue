<template>
  <div>
    <v-app-bar id="home" app color="transparent" :hide-on-scroll="true" flat>
      <v-btn text large>Juris</v-btn>
      <v-spacer></v-spacer>
      <v-btn text small color="white">
        Sobre
      </v-btn>
      <v-btn text small color="white">Como usar</v-btn>
      <v-btn text small color="white">Serviços</v-btn>
      <v-btn text small color="white">FAQ</v-btn>
      <v-btn text small color="white">Contato</v-btn>
      <v-btn large color="primary">Login</v-btn>
    </v-app-bar>
    <v-main>
      <v-lazy>
        <v-container class="vContainer">
          <v-card id="vCard" color="transparent" outlined width="35%">
            <p id="cardText">
              Torne o seu fluxo <br />
              de atendimento aos seus clientes <br />
              mais simples
            </p>
            <v-card-actions>
              <v-btn color="primary" large rounded> Contrate agora </v-btn>
            </v-card-actions>
          </v-card>
        </v-container>
      </v-lazy>
      <v-lazy>
        <v-container class="vContainer">
          <div class="about">
            <h1>This is an about page</h1>
          </div>
        </v-container>
      </v-lazy>
    </v-main>
  </div>
</template>

<script>
export default {
  name: "Home",
};
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
</style>
