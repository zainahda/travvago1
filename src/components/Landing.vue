<template>
  <div>
    <b-jumbotron class="jumbotron">
      <div class="container">
        <p class="animate__animated animate__fadeInDown animate__slower" id="display-4">
          Temukan hal-hal menakjubkan <br />
          untuk dilakukan Kapan saja, dimana saja.
        </p>
        <div></div>
        <b-button size="lg" class="button my-2 my-sm-0 animate__animated animate__fadeInUp animate__slower" type="submit"
          >Explore Now</b-button
        >
      </div>
    </b-jumbotron>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Permanent+Marker&display=swap");

.jumbotron {
  background-image: url(../assets/bg3.jpg);
  background-size: cover;
  height: 682px;
  text-align: center;
  position: relative;
}
.jumbotron .container {
  z-index: 1;
  position: relative;
}
.jumbotron::after {
  content: "";
  display: block;
  width: 100%;
  height: 100%;
  background: linear-gradient(
    180deg,
    rgba(29, 116, 248, 0.5) 0%,
    rgba(0, 0, 0, 0.125) 100%
  );
  position: absolute;
  bottom: 0;
  left: 0;
}
.jumbotron,
#display-4 {
  font-size: 36px;
  font-family: "Permanent Marker", cursive;
  color: white;
  line-height: 52px;
  text-shadow: 0px 4px 4px rgba(0, 0, 0, 0.75);
}
#display-4 {
  margin-top: 150px;
  text-shadow: 0px 4px 4px #f85e1d;
}
.jumbotron .btn {
  color: white;
}
.btn {
  margin-top: 10px;
}
.button:active {
  position: relative;
  top: 7px;
  box-shadow: none;
}
.button {
  background: linear-gradient(180deg, #fea858 0%, #f85e1d 100%);
  box-shadow: inset 0px 4px 4px rgba(0, 0, 0, 0.25);
}

/* Desktop Version */
@media (min-width: 992px) {
  .jumbotron {
    margin-top: -100px;
    height: 782px;
  }
  #display-4 {
    margin-top: 360px;
  }
  .btn {
    margin-top: 0;
  }
}
</style>