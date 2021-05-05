<template>
  <v-content>
    <div class="staticHero">
      <v-img src="../assets/images/img13.jpg">
        <v-row align="end" class="lightbox white--text pa-2 fill-height">
          <v-col>
            <v-container>
              <div class="headline">Cv video </div>
            </v-container>
          </v-col>
        </v-row>
      </v-img>
    </div>
    <div class="block">
      <v-container>
        <p>Mit navn er <strong>Dustin Chwalek.</strong> Og er blevet opmærksom på jeres stilling opslag via  
Erhversakademiets egen jobportal. Stilling tiltager mig på mange punkter. Der jeg beskriver mig som en ildsjælet og arrangeret person, som angår projekterne planlagt og målrettet. Jeg giver altid 110 procent i alle forskelllige størrelser af projekter, og lever af erfaringerer, såvel mislykken og succes momenter. Jeg vil beskrive mig som en loyalt og energisk medarbejder.
Jeg er pt ansat som tilkalds vikar på et bosted, dog vægter jeg studieorientering og ønsker et dybere indblik omkring arbejde som multimediedesigner og de udfordringer. Fritiden bruger jeg stort set på at dyrke motionen, eller at opleve naturen. </p>
      </v-container>
    </div>
    <div class="block">
      <v-container>
        <h2 class="text-center">Mine kompetencer</h2>
        <v-row>
          <v-col v-for="item in items" :key="item.id" class="d-flex child-flex" cols="12" sm="4">
            <v-card flat tile class="mx-auto">
              <v-img :src="item.src" aspect-ratio="1" class="grey lighten-2"></v-img>
              <v-card-text class="text--primary text-center">
                <div class="title">{{ item.name }}</div>
                <p>{{ item.title }}</p>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
  
<section>
      <div class="youtube">
      <iframe width="560" height="315" src="https://www.youtube.com/embed/QqvpGUWuQrE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div>
    </section>
</v-content>
</template>

<script>
export default {
  name: "About",
  data() {
    return {
      items: [
        {
          id: 1,
          src: require("../assets/images/team1.jpg"),
          name: 'Adobe',
          title: 'Redigeringsprogrammer '
        },
        {
          id: 2,
          src: require("../assets/images/team2.jpg"),
          name: 'User Experimence',
          title: 'Undersøgelses Design'
        },
        {
          id: 3,
          src: require("../assets/images/team3.jpg"),
          name: 'Dustin Chwalek',
          title: 'Multimedia Design'
        }
      ]
    };
  }
};
</script>

<style lang="scss">

.youtube {
  display: flex;
  justify-content: center;
  padding-bottom: 20px;
}

</style>