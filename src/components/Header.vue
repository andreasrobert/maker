<template>
<div>
 <img src="../assets/logo.svg" />
</div>
</template>


<style scoped>
 div {
     padding: 20px 0px 40px 0px;
     width: 85% ;
     display: flex;
 }


 img{
     width: 120px;
     height: 35px;
     margin: 20px 0px 20px 0px;
 }

 @media only screen and (max-width: 1200px) {
  div {
    width:100%;
    padding:15px 0px 30px 70px
  }
}
 @media only screen and (max-width: 515px) {
  div {
    display: flex;
    justify-content: center;
    padding: 10px 0px 10px;
  }
}

</style>