<template>
  <v-app>
    <v-container id="app">
      <ImageLog />
      <Botao icon="whatsapp" msg="Whatsapp" />
      <Botao icon="instagram" msg="Instagram" />
      <Botao icon="drive" msg="Google Drive" />
      <Frases />
    </v-container>
    <!-- <v-dialog v-model="dialog" width="358">
      <v-row>
        <v-card>
          <v-card-title class="headline grey lighten-2" primary-title>Bem vindo a Sherlock Imports!</v-card-title>
          <v-divider></v-divider>
        </v-card>
      </v-row>
    </v-dialog>-->
  </v-app>
</template>

<script>
import ImageLog from "./components/ImageLog";
import Botao from "./components/Botoes";
import Frases from "./components/Frases";

export default {
  data() {
    return {
      enter: true,
      dialog: true
    };
  },
  components: {
    ImageLog,
    Botao,
    Frases
  }
  /* mounted() {
    setTimeout(() => {
      this.dialog = false;
    }, 2000);
  } */
};
</script>

<style>
#app {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 100vh;
  font-size: 1.6rem;
  background-image: url("./images/background.jpg");
}
</style>