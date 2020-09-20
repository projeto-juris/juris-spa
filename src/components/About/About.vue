<template>
  <v-container class="vContainer">
    <v-row no-gutters>
      <v-col md="4">
        <v-card flat class="card">
          <v-row>
            <v-col md="1">
              <settings-icon size="1.5x" class="icons"></settings-icon>
            </v-col>
            <v-col md="11">
              <v-card-text>
                Assistante Virtual Juridico Personalizavel
              </v-card-text>
              <v-card-subtitle>Personalizavel</v-card-subtitle>
            </v-col>
          </v-row>
        </v-card>
      </v-col>
      <v-col md="5">
        <v-card flat class="card">
          <v-row>
            <v-col md="1">
              <shield-icon size="1.5x" class="icons"></shield-icon>
            </v-col>
            <v-col md="11">
              <v-card-text>
                Os dados do seus clientes com a proteção da nova leiLGPD
              </v-card-text>
              <v-card-subtitle>Segurança</v-card-subtitle>
            </v-col>
          </v-row>
        </v-card>
      </v-col>
      <v-col md="3">
        <v-card flat class="card">
          <v-row>
            <v-col md="1">
              <clock-icon size="1.5x" class="icons"></clock-icon>
            </v-col>
            <v-col md="11">
              <v-card-text>Disponivel a qualquer hora e lugar</v-card-text>
              <v-card-subtitle>Praticidade</v-card-subtitle>
            </v-col>
          </v-row>
        </v-card>
      </v-col>
    </v-row>
    <v-row>
      <v-spacer />
      <v-col md="3">
        <h1>COMO UTILIZAR</h1>
      </v-col>
      <v-spacer />
    </v-row>
    <v-row>
      <v-spacer />
      <v-col md="3">
        <v-card elevation="5" style="margin: 5px;">
          <v-list-item three-line>
            <v-list-item-content>
              <v-card-subtitle>Passo 1</v-card-subtitle>
              <v-list-item-title class="listItemTitle"
                >Procure pelo botão
              </v-list-item-title>
              <v-card-subtitle style="font-size: 12px; color: black;">
                No canto inferior direito da pagina encontra-se um botão azul,
                clique no botão para começar.
              </v-card-subtitle>
            </v-list-item-content>
          </v-list-item>
        </v-card>
        <v-card flat disabled>
          <v-list-item three-line>
            <v-list-item-content>
              <v-card-subtitle class="overline">Passo 2</v-card-subtitle>
              <v-list-item-title class="listItemTitle"
                >Entre com seu identificador
              </v-list-item-title>
              <v-card-subtitle>
                Dentro da conversa de chat, insira o seu identificador pessoal.
              </v-card-subtitle>
            </v-list-item-content>
          </v-list-item>
        </v-card>
        <v-card flat disabled>
          <v-list-item three-line>
            <v-list-item-content>
              <v-card-subtitle class="overline">Passo 3</v-card-subtitle>
              <v-list-item-title class="listItemTitle"
                >Escolha uma das funções
              </v-list-item-title>
              <v-card-subtitle>
                Escolha uma das funções que desejar clicando no botão desejado.
              </v-card-subtitle>
            </v-list-item-content>
          </v-list-item>
        </v-card>
      </v-col>
      <v-col md="7">
        <v-img src="../../assets/chats.png" id="img" />
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
import { SettingsIcon, ShieldIcon, ClockIcon } from "vue-feather-icons";
export default {
  components: {
    SettingsIcon,
    ShieldIcon,
    ClockIcon,
  },
};
</script>
<style scoped>
.icons {
  stroke-width: 1px;
}
.v-card__text {
  font-size: 14px;
  font-weight: bold;
  line-height: 30px;
  color: black !important;
  padding: 0px;
}
.v-card__subtitle {
  padding: 0;
}
h1 {
  font-weight: 300;
  letter-spacing: 3px;
}
.listItemTitle {
  font-size: 18px;
  padding: 3px;
  color: #03293b;
}
#img {
  max-width: 55vh;
}
</style>
