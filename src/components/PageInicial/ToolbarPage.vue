<template>
  <div>
    <v-app-bar style="height: 100px; width: auto;" color="blue">
      <v-app-bar-nav-icon @click="drawer = !drawer" class="nav"></v-app-bar-nav-icon>
      <v-spacer></v-spacer>
      <v-toolbar-title class="text-center; ">
        <img src="../../images/1.png" class="icon">
      </v-toolbar-title>
      <v-spacer></v-spacer>
    </v-app-bar>

    <v-navigation-drawer color="blue" v-model="drawer" app temporary>
      <v-list color="rgb(35, 65, 147)" class="rounded-b-lg">
          <v-card-title class="bg-sky-600 w-2/4 flex justify-center ml-15 mb-3  rounded-md">
            MENU
          </v-card-title>
        <v-list-item>
          <v-list-item-content>
            <v-btn @click="currentPage = 'home', drawer = false" color="blue" style="width: 90%;">Home</v-btn>
          </v-list-item-content>
        </v-list-item>
        <v-list-item>
          <v-list-item-content>
            <v-btn @click="currentPage = 'about', drawer = false" color="blue" style="width: 90%;">Sobre o Partido</v-btn>
          </v-list-item-content>
        </v-list-item>
        <v-list-item>
          <v-list-item-content>
            <v-btn  @click="currentPage = 'contact', drawer = false" color="blue" style="width: 90%;">Proposta de Governo</v-btn>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <app-homepage v-if="currentPage === 'home'"></app-homepage>

    <app-alternativeconteudo v-if="currentPage === 'about'"></app-alternativeconteudo>

    <app-home-propostas v-if="currentPage === 'contact'"></app-home-propostas>
  </div>
</template>

<script>
import HomePropostas from '../Propostas.vue/HomePropostas.vue';
import HomePage from './HomePage.vue';
import MorePartido from '../SobrePartido.vue/MorePartido.vue';

export default {
  components: {
    'app-homepage': HomePage,
    'app-alternativeconteudo': MorePartido,
    'app-home-propostas': HomePropostas,
  },

  data() {
    return {
      drawer: false,
      currentPage: 'home'
    }
  },
}
</script>

<style>
.nav-enter-active, .nav-leave-active {
  transition: opacity 0.5s;
}

.nav-enter, .nav-leave-to {
  opacity: 0;
}


.text-menu {
  font-size: 70px,
}

.menu {
  margin-left: 20px;
  width: 85%;
  height: 40px;
  border-radius: 10px;
  background-color: navy;
  text-align: center;
  color: rgb(235, 235, 232);
}

.icon {
  margin-right: 20px;
  margin-top: 40px;
  height: 120px;
}

.nav {
  background-color: rgb(38, 104, 190);
  border-radius: 10px;
  margin-left: 30px;
  margin-top: 40px;
}

teste {
  background-color: rgb(88, 86, 175);
}
</style>
