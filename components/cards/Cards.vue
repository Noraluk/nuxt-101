<template>
  <v-item-group>
    <v-container fluid>
      <v-row>
        <v-col v-for="n in 8" :key="n" cols="12" md="6">
          <v-card class="px-5 pt-5">
            <br />
            <v-card-title class="card-title"> Another headline </v-card-title>
            <v-card-text class="card-text">
              And an even wittier subheading.
            </v-card-text>
            <br />
            <v-card dark height="400" class="card-inside"> </v-card>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-item-group>
</template>

<style scoped>
.card-title {
  font-size: 45px;
  font-weight: normal;
  justify-content: center;
}

.card-text {
  font-size: 20px;
  justify-content: center;
  text-align: center;
}

.card-inside {
  margin-left: 50px;
  margin-right: 50px;
  border-radius: 30px 30px 0px 0px;
}
</style>
