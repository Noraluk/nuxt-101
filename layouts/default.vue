<template>
  <v-app>
    <v-app-bar :clipped-left="clipped" fixed app flat color="#212529">
      <v-container>
        <v-row no-gutters>
          <v-col>
            <v-icon color="grey">fa-carrot</v-icon>
          </v-col>
          <v-col v-for="n in menus.length" :key="n" class="menu">
            <NuxtLink class="menu" to="/">{{ menus[n - 1] }}</NuxtLink>
          </v-col>
        </v-row>
      </v-container>
    </v-app-bar>
    <v-main>
      <Nuxt />
    </v-main>
    <v-footer :absolute="!fixed" app>
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      menus: [
        "Tour",
        "Product",
        "Features",
        "Enterprise",
        "Support",
        "Pricing",
        "Cart",
      ],
    };
  },
};
</script>

<style scoped>
.v-application {
  background-color: white;
}

.col {
  text-align: center;
}

.menu {
  color: #8e8e8e;
  font-size: 20px;
}
</style>
