<template>
  <div id="welcome">
    <div class="hello">
      <h2>Hello! <br>I'm Ramona Oviatt</h2>
      <div class="helloImgs">
        <!-- <img src="../assets/duck.svg" alt="A cartoon cat" /> -->
        <img src="../assets/export.png" alt="A cartoon ramona" />

        <!-- <img src="../assets/tuco.svg" alt="A cartoon dog" /> -->
      </div>

      <welcome-text></welcome-text>
    </div>
  </div>
</template>

<script>
import WelcomeText from "./WelcomeText.vue";
export default {
  components: { WelcomeText },
  name: "welcome-container",
};
</script>

<style lang="scss" scoped>
#welcome {
  display: grid;
  place-items: center;
}
.helloImgs {
  display: grid;
  place-items: center;
  background: #EFEFD2;
  border-radius: 50%;
  height: 170px;
  width: 170px;
  // grid-template-columns: 1fr 1fr 1fr;
  // height: 100px;
  // width: 29px;


  img {
    height: 140px;
    margin-right: -6px;
    // position: absolute;
  // transform: sc;
  //   width: 30%;
  //   right: 35%;
  //   left: 35%;
  }
}
h2 {
  margin-bottom: 30px;
}
.hello {
  display: grid;
  place-items: center;
  margin-top: 110px;
  
  h2 {
   
    text-align: center;
  }
  
}

// @media screen and (min-width: 320px) {
//   .helloImgs {
//     width: 70%;
//     margin: 30px 0;
//     display: grid;
//     place-items: center;
//     grid-template-columns: 1fr 1fr 1fr;
//     height: 100px;
//     :nth-child(2) {
//       height: 100px;
//       margin-bottom: 90px;
//     }
//     :nth-child(3) {
//       transform: scaleX(-1);
//       z-index: -1;
//     }

//     img {
//       height: 70px;
//     }
//     .waves {
//       display: none;
//     }
//   }
// }

@media screen and (min-width: 500px) {
  
  #welcome {
    margin-top: 130px;
  }
}
.techPets {
  width: 60%;
}
</style>