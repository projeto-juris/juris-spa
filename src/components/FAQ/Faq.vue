<template>
  <v-container style="margin-top: 300px">
    <v-spacer />
    <v-row>
      <v-col cols="8">
        <v-row align="start" justify="start">
          <h1>PERGUNTAS FREQUENTES</h1>
        </v-row>
        <v-row align="start" justify="start">
          <div class="vList">
            <v-list>
              <v-list-group no-action disabled>
                <template v-slot:activator>
                  <plus-circle-icon size="1.5x" class="icons"></plus-circle-icon>
                  <v-list-item-content>
                    <v-list-item-title>Eu posso personalizar minha agenda?</v-list-item-title>
                  </v-list-item-content>
                </template>
              </v-list-group>
              <v-list-group no-action @click="changeIcon">
                <template v-slot:activator>
                  <plus-circle-icon v-show="!iconActive" size="1.5x" class="icons"></plus-circle-icon>
                  <minus-circle-icon v-show="iconActive" size="1.5x" class="activeIcon"></minus-circle-icon>
                  <v-list-item-content>
                    <v-list-item-title>Como Juris pode me ajudar em minha relação diária com os clientes?</v-list-item-title>
                  </v-list-item-content>
                </template>
                <v-list-item>
                  <v-list-item-content>
                    <v-list-item-text>
                      O Juris é o seu Assistente Virtual que está disponivel
                      para seus clientes a qualquer hora do dia, basta ele fazer uma pergunta ao
                      Juris e ele tira todas as duvidas dos seus clientes.
                    </v-list-item-text>
                  </v-list-item-content>
                </v-list-item>
              </v-list-group>
              <v-list-group no-action disabled>
                <template v-slot:activator>
                  <plus-circle-icon size="1.5x" class="icons"></plus-circle-icon>
                  <v-list-item-content>
                    <v-list-item-title>Porque usar o Juris ?</v-list-item-title>
                  </v-list-item-content>
                </template>
              </v-list-group>
            </v-list>
          </div>
        </v-row>
      </v-col>
    </v-row>
    <v-spacer />
  </v-container>
</template>
<script>
import { PlusCircleIcon, MinusCircleIcon } from "vue-feather-icons"

export default {
  data() {
    return {
      iconActive: false,
    }
  },
  components: {
    PlusCircleIcon,
    MinusCircleIcon,
  },
  methods: {
    changeIcon() {
      this.iconActive = !this.iconActive
      console.log(this.iconActive)
    },
  },
}
</script>
<style>
.vList {
  width: 100%;
}
.icons {
  border-radius: 20px;
  stroke-width: 1.5px;
  background-color: #03293b;
  color: white;
  margin-right: 5px;
}
.activeIcon {
  color: #03293b;
  stroke-width: 1px;
  margin-right: 5px;
}
</style>