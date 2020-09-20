<template>
  <v-container class="vContainer">
    <v-row>
      <v-col>
        <settings-icon size="1.5x" class="custom-class"></settings-icon>
      </v-col>
      <v-col> </v-col>
      <v-col> </v-col>
    </v-row>
  </v-container>
</template>
<script>
import { SettingsIcon } from "vue-feather-icons";
export default {
  components: {
    SettingsIcon,
  },
};
</script>
