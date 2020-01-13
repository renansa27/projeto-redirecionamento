<template>
  <div>
    <v-col>
      <v-btn min-width="170" outlined color="black">
        <v-row class="rowBtn">
          <div></div>
          {{msg}}
          <img class="img" :src="getUrl()" />
        </v-row>
      </v-btn>
    </v-col>
  </div>
</template>

<script>
import wppIcon from "../images/whatsapp.png";
import instagramIcon from "../images/instagramIcon.png";
import youtube from "../images/youtube.png";
import fbIcon from "../images/facebook.png";
import drive from "../images/drive.png";

export default {
  data() {
    return {};
  },
  props: {
    msg: String,
    icon: String
  },
  methods: {
    getUrl() {
      if (this.icon == "whatsapp") {
        return wppIcon;
      } else if (this.icon == "instagram") {
        return instagramIcon;
      } else if (this.icon == "youtube") {
        return youtube;
      } else if (this.icon == "drive") {
        return drive;
      } else {
        return fbIcon;
      }
    }
  }
};
</script>

<style>
.rowBtn {
  justify-content: space-between;
  align-items: center;
}
.img {
  justify-content: end;
  width: 24px;
  height: 24px;
}
</style>