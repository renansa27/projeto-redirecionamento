<template>
  <div>
    <v-card class="tam">
      <v-img :aspect-ratio="7/9" :src="img" class="trasparent"></v-img>
      <v-card-title>Sherlock Imports</v-card-title>
    </v-card>
  </div>
</template>

<script>
import imgStartUp from "../images/newLogo.png";

export default {
  data() {
    return {
      img: imgStartUp
    };
  }
};
</script>

<style>
.transparent {
  border-color: transparent !important;
}

.tam {
  background-color: transparent !important;
  border-color: transparent !important;
}
.text {
  justify-content: center;
}
</style>