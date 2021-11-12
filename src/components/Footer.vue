<template>
  <div class="container">
    <h1 class="sBold">Get notified when we launch</h1>
    <div class="form">
      <input type="text" placeholder="email address" />
      <button>Get notified</button>
    </div>
  </div>
</template>

<style scoped>
h1 {
  margin: 0 0 20px;
}
.container {
  margin-bottom: 100px;
  width: 100%;
  height: 200px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  background-image: url(../assets/bg-footer-squiggle.svg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
}

input {
  border: none;
  outline: none;
  color: white;
  font-weight: 800;

  width: 280px;
  padding: 20px;
  height: 8px;
  border-radius: 25px;
  background-color: #093f68;
  margin-right: 20px;
}

button {
  all: unset;
  cursor: pointer;
  font-weight: 800;
  padding: 10px;
  border-radius: 25px;
  background-color: #3ee9e5;
  border: 1px solid #3ee9e5;
  color: #093f68;
}

button:hover {
  background-color: #080c20;
  border: 1px solid #3ee9e5;
  color: #3ee9e5;
}

::placeholder { 
  color: #777f98;
  opacity: 1; /* Firefox */
}

@media only screen and (max-width: 515px) {
  .form{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  h1{
    font-size: 24px;
  }
  button{
    width: 100%;
    padding: 10px 0px 10px 0px;
  }

  input{
    margin: 0px 0px 20px 0px;
    width: 70vw;
  }
}


</style>
