<template>
  <div class="block latestPostBlock">
    <v-container>
      <h2 class="text-center">Education</h2>
      <v-row>
        <v-col v-for="item in items" :key="item.id" cols="12" md="4">
          <v-card outlined class="mx-auto">
            <v-img
              class="white--text align-end"
              height="200px"
              :src="item.src"
            >
              <v-card-title>{{ item.title }}</v-card-title>
            </v-img>
            <v-card-subtitle class="pb-0">{{ item.subtitle }}</v-card-subtitle>
            <v-card-text class="text--primary">
              <div>{{ item.description }}</div>
            </v-card-text>
            <v-card-actions>
              <v-btn color="primary" text>More</v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  name: "LatestPost",
  data: () => ({
    show: false,
    items: [
      {
        id: 1,
        title: "Syddansk universitet",
        subtitle: "informationsvidenskab it og interaktionsdesign",
        description: "Læring omkring programmer, desing og analysere hjemmesider og interaktive produkter, med udgangspunkt i forståelse af mennesker .",
        src: require("../assets/images/img10.jpg")
      },
      {
        id: 2,
        title: "Ribe Katedralskole",
        subtitle: "Højere forberedelseseksamen",
        description: "HF Dansk A Engelsk B Matematik C Kultur- og samfundsfaggruppe: historie B, religion C, samfundsfag C Billedkunst,Psykolog,Tysk A .",
        src: require("../assets/images/img11.jpg")
      },
      {
        id: 3,
        title: "E r h v e r s         A k a d e m i         S y d v e s t ",
        subtitle: "Multimedia designer",
        description: "Mit multimedia mindeset gør mig unikt omkring design og digitale løsningerne. At udvikling og design af både af hjemmesider, eller projekter-.",
        src: require("../assets/images/img12.jpg")
      }
    ]
  })
};
</script>