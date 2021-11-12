<template>
  <div class="container">
    <div class="box passion">
      <div class="pic">
        <img src="../assets/illustration-passions.svg" alt="" />
      </div>
      <div class="detail">
        <h1 class="xMedium">Indulge your passions</h1>
        <p class="medium">
          Your passions shouldn't be just for the weekend. Earn a living doing
          what you love.
        </p>
      </div>
    </div>

    <div class="box freedom">
      <div class="pic">
        <img src="../assets/illustration-financial-freedom.svg" alt="" />
      </div>
      <div class="detail">
        <h1 class="xMedium">Gain financial freedom</h1>
        <p class="medium">
          Start making money work for you. There's nothing quite like earning
          while you sleep
        </p>
      </div>
    </div>

    <div class="box life">
      <div class="pic">
        <img src="../assets/illustration-lifestyle.svg" alt="" />
      </div>
      <div class="detail">
        <h1 class="xMedium">Choose your lifestyle</h1>
        <p class="medium">
          Own your daily schedule. Fancy a lie-in? Go for it! Take charge of
          your week.
        </p>
      </div>
    </div>

    <div class="box anywhere">
      <div class="pic">
        <img src="../assets/illustration-work-anywhere.svg" alt="" />
      </div>
      <div class="detail">
        <h1 class="xMedium">Work from anywhere</h1>
        <p class="medium">
          Selling online means not being pinned down. Want to work AND travel?
          Go for it!
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  text-align: left;
  padding-bottom: 150px;

  /* background-color: aquamarine; */
  justify-content: space-between;
  width: 80%;
}

.box {
  width: 255px;
  height: 335px;
}
.pic {
  width: 160px;
  height: 164px;
  background-color: #093f68;
  border-radius: 30%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 45px;
}

.freedom,
.anywhere {
  margin-top: 50px;
}

.passion,
.freedom,
.life {
  margin-right: 50px;
}

.medium {
  font-weight: 500;
  font-size: 0.8vw;
  color: #777f98;
  line-height: 1.5vw;
  margin: 0px;
}

@media only screen and (max-width: 1200px) {
  .medium {
    font-size: 1.3vw;
  }
}

@media only screen and (max-width: 1000px) {
  .medium {
    font-size: 15px;
    line-height: initial;
    width: 30vw;
  }
  .container {
    flex-direction: column;
  }
  .box {
    display: flex;
    width: 100%;
    height: 100%;
    margin: 0 0 40px;
  }
  .pic {
    margin: 0 55px 0px 0px;
    min-width: 160px;
  }

  .detail {
    display: flex;
    justify-content: center;
    flex-direction: column;
  }

  .passion,
  .life {
    margin-left: 58px;
  }
}

@media only screen and (max-width: 800px) {
  .container {
    width: 90%;
  }
}

@media only screen and (max-width: 515px) {
  .box {
    display: flex;
    flex-direction: column;
    margin: 0px 0px 50px 0px;
    align-items: center;
    text-align: center;
  }

  .pic {
    margin: 0px 0px 10px 0px;
  }
  .container {
    padding: 0px 0px 10px 0px;
  }

  .medium {
    width: 80%;
  }
  .detail{
    align-items: center;
    
  }

}
</style>
