<template>
  <div class="header">
    <h1>Our pricing plans</h1>
    <p>
      We only make money when our creators make money. Our plans are always
      affordable, and it’s completely free to get started.
    </p>
  </div>
  <div class="content">
    <div class="box left">
      <img class="logo" src="../assets/icon-free.svg" alt="" />
      <h1>Dip your toe</h1>
      <p>
        Just getting started? No problem at all! Our free plan will take you a
        long way.
      </p>
      <h1>Free</h1>
      <div class="list" v-for="feat in free" :key="feat">
      <img class="check leftCheck" src="../assets/icon-check.svg" alt="" />
      <p>{{feat}}</p>
      </div>
    </div>
    <div class="box right">
      <img class="logo" src="../assets/icon-paid.svg" alt="" />
      <h1>Dive right in</h1>
      <p>
        Ready for the big time? Our paid plan will help you take your business
        to the next level.
      </p>
      <div class="money">
        <h1>$25.00</h1>
        <p>/month</p>
      </div>
         <div class="list" v-for="feat in paid" :key="feat">
      <img class="check" src="../assets/icon-check.svg" alt="" />
      <p>{{feat}}</p>
      </div>
      
    </div>
  </div>
</template>

<script>
export default {
    data(){
        return{
            free:[
                "Unlimitied products",
                "Basic analytics",
                "Limited marketplace expsure",
                "10% fee per transaction"
            ],
            paid:[
                "Custome domain",
                "Advanced analytics and reports",
                "High marketplace visibility",
                "5% fee per transaction",
            ]
        }
    }
}
</script>

<style scoped>
.left {
  height: 349px;
  background-color: #093f68;
  margin-right: 30px;
}

.right {
  height: 373px;
  background-color: #3ee9e5;
  color: #080C20 !important;
}

.box {
    position: relative;
  width: 369px;
  border-radius: 12px;
  display: flex;
  flex-direction: column;
  text-align: left;
  align-items: flex-start;
  padding: 38px;
}

.logo{
    position: absolute;
    top: -23px;
}

.right img{
    top: -35px;
}

.right h1{
    color:#080C20
}

.money{
    display: flex;
    align-items: center;
}

.content{
    display: flex;
    justify-content: center;
    align-items: center;
    padding-bottom: 240px;

}

.header{
    margin-bottom: 58px;
}

.list{
    display: flex;
    align-items: center;
}

.check{
    width: 15px;
    height: 15px;
    margin-right: 10px;
}

.leftCheck{
    filter: invert(80%) sepia(89%) saturate(1289%) hue-rotate(142deg) brightness(91%) contrast(100%);
}

.list p{
    margin: 1px 0px;
}

@media only screen and (max-width: 1000px) {
  .content {
      flex-direction: column;
  }
  .left {
  height: 349px;
  background-color: #093f68;
  margin: 0px 0px 80px 0px;
}
.header{
    width: 80%;
}
}

@media only screen and (max-width: 515px) {
  .content {
      padding: 0px 0px 50px 0px;
  }
  .left {

}
.header{
}

.box{
    width: 70vw;
}
}

</style>
