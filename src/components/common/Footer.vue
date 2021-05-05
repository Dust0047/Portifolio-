<template>
  <v-container>
    <v-footer padless>
      <v-card flat class="text-center">
        <v-card-text>
          <v-btn v-for="icon in icons" :key="icon" class="mx-4" icon>
            <v-icon size="24px">{{ icon }}</v-icon>
          </v-btn>
        </v-card-text>
        <v-card-text
          class="pt-0"
        >Download mit fulde Cv. Med værker udarbejdet i 2021 med balandt andet logo design og meget mere Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nostrum quae quasi placeat fugit reprehenderit dolorum in voluptatum at error nisi vel facere ipsa eveniet quo laborum, ullam odit eum facilis?</v-card-text>
        <v-divider></v-divider>
         <v-btn 
      id="button"
      elevation="2"
      color="green">
      <a href="https://erhvervsakademisydvest-my.sharepoint.com/:b:/g/personal/dust0047_easv365_dk/EXavjvpUPS1EpqjWJRL6AXwBGjTm-1mZ4krGDc0RA3U9yA?e=N8te6g" target="_blank">
      Download
      </a>
      </v-btn>
        <v-card-text>
          {{ new Date().getFullYear() }} —
          <strong>Photography Vuetify Project</strong>
        </v-card-text>
      </v-card>
    </v-footer>
  </v-container>
</template>

<script>
export default {
  name: "Header",
  data: () => ({
    icons: [
      "fab fa-facebook",
      "fab fa-twitter",
      "fab fa-google-plus",
      "fab fa-linkedin",
      "fab fa-instagram"
    ]
  })
};
</script>