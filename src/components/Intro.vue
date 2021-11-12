<template>
  <div class="container">
    <div class="mobile"></div>
    <img src="../assets/illustration-hero-left.svg" alt="" />

    <div class="message">
      <h1 class="xBold">Get paid for the work</h1>
      <h1 class="xBold blue">love</h1>
      <p class="medium">
        The 9 - 5 grind is so last century. We believe in living life on your
        own terms. Wheter you're looking to escape the rat race or set up a side
        hustle. We've got you covered
      </p>

      <img class="scroll" src="../assets/icon-scroll.svg" alt="" />
    </div>

    <img  src="../assets/illustration-hero-right.svg" alt="" />
  </div>
</template>

<style scoped>
.container {
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: space-between;
  margin-bottom: 180px;
  /* background-color: #3ee9e5; */
}

.message {
  display: flex;
  flex-direction: column;
  justify-content: center;
  width: 100%;
  max-height: 30vw;
  align-items: center;
  background-image: url(../assets/bg-hero-squiggle.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
}

.blue {
  color: #3ee9e5;
}
.blue::after {
  color: white;
  content: " to do";
}
.blue::before {
  color: white;
  content: "you ";
}

.medium {
  max-width: 540px;
}

h1 {
  margin: 0px;
}

img {
  height: 30vw;
}

.scroll {
  margin-top: 2vw;
  width: initial;
  height: initial;
}

@media only screen and (max-width: 515px) {
  h1{
    font-size: 32px;

  }

  p{
    font-size: 15px;
    width: 90%;
  }
  .container {
    flex-direction: column;
    justify-content: space-between;
    margin-bottom: 80px;
  }
  img{
    display: none;
  }

  .mobile{
      background-image: url(../assets/illustration-hero-mobile.png);
  background-repeat: no-repeat;
  background-position: center;
  background-size: contain;
    height: 250px;
    margin-bottom: 25px;

  }

  .message{
    max-height: initial;
  }

  .scroll {
  display: initial;
}
}
</style>
