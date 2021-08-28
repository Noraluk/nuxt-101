<template>
  <div>
    <v-container fluid class="banner">
      <div class="col-md-5 mx-auto div-inside">
        <p class="title-banner">Punny headline</p>
        <p class="body-banner">
          And an even wittier subheading to boot. Jumpstart your marketing
          efforts with this example based on Apple’s marketing pages.
        </p>
        <v-btn class="ma-2" outlined color="grey"> Coming soon </v-btn>
      </div>
      <div class="product-device" />
      <div class="product-device product-device-2" />
    </v-container>
  </div>
</template>

<style>
.banner {
  position: relative;
  overflow: hidden;
  display: block;
  background-color: #f8f9fa;
  text-align: center;
  margin: 16px;
  padding: 48px;
}

.banner-button {
  width: 100px;
}

.div-inside {
  margin-top: 40px;
  margin-bottom: 40px;
  padding-top: 100px;
  padding-bottom: 100px;
}

.product-device {
  position: absolute;
  right: 10%;
  bottom: -30%;
  width: 350px;
  height: 640px;
  background-color: #333;
  border-radius: 21px;
  transform: rotate(30deg);
  box-shadow: 0 0.125rem 0.25rem rgba(0, 0, 0, 0.075) !important;
}

.product-device-2 {
  top: -25%;
  right: auto;
  bottom: 0;
  left: 5%;
  background-color: #e5e5e5;
}

.product-device::before {
  position: absolute;
  top: 10%;
  right: 10px;
  bottom: 10%;
  left: 10px;
  content: "";
  background-color: rgba(255, 255, 255, 0.1);
  border-radius: 5px;
}

.title-banner {
  font-size: 55px;
  font-weight: 500;
}

.body-banner {
  font-size: 1.25rem;
  font-weight: 500;
}
</style>
