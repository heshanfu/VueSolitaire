<template>
  <div class="page_wrapper">
    <div class="heading">
      <a href="http://github.com/silent-lad/VueSolitaire"
        ><img src="../assets/sl.png" alt="silentlad" class="logo"
      /></a>

      <h1>
        VueSolitaire
      </h1>
    </div>

    <div class="menu_wrapper">
      <router-link to="/klondike">
        <div class="option">
          <img src="../assets/images/3.png" alt="" srcset="" />

          <p>Klondike Solitaire</p>
        </div>
      </router-link>

      <router-link to="/spider/1">
        <div class="option larger">
          <img src="../assets/images/1.png" alt="" srcset="" />
          <p>Spider Solitaire</p>
        </div>
      </router-link>

      <router-link to="/spider/2">
        <div class="option">
          <img src="../assets/images/5.png" alt="" srcset="" />
          <p>Spider Solitaire [2 Suit]</p>
        </div>
      </router-link>
    </div>
  </div>
</template>
<script>
export default {};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Pacifico");
.logo {
  margin: 1% 0 0 0;
  height: 70px;
  padding: 5px;
  background: white;
  border-radius: 5px;
  box-shadow: 2px 2px 10px black;
}
h1 {
  margin: 0 0 0 0;
  color: rgb(34, 34, 32);
  font-weight: 400;
  font-family: "Pacifico", cursive;
  font-size: 50px;
  text-shadow: 3px 2px 4px rgba(0, 0, 0, 0.548);
}
.page_wrapper {
  text-align: center;
  background-image: radial-gradient(
    rgba(57, 172, 57, 0.726),
    rgb(0, 116, 0),
    darkgreen
  );
  height: 100vh;
  overflow: hidden;
}
.menu_wrapper {
  /* margin: 0; */
  display: flex;
  flex-direction: row;
  justify-content: space-around;
}
.option img {
  transition: all 0.3s;
  margin: 5%;
  width: 80%;
  padding: 5%;
  border: 2px solid lightblue;
  border-radius: 10px;
}
.option p {
  color: darkred;
  text-align: center;
  font: 40px Georgia, Times New Roman, serif;
}

.option {
  position: relative;
  top: 10vh;
  background: rgb(34, 34, 32);
  border-radius: 10px;
  width: 25vw;
  height: 50vh;
  -webkit-box-shadow: 3px 3px 7px rgba(0, 0, 0, 0.3);
  box-shadow: 3px 3px 7px rgba(0, 0, 0, 0.3);
  padding: 4%;
}
.larger {
  transform: scale(1.1, 1.1);
}

.option:hover {
  transition: all 0.3s;
  transform: scale(1.2, 1.2);
  border: 3px solid firebrick;
  box-shadow: 10px 10px 10px rgba(0, 0, 0, 0.8);
}
.option:hover p {
  color: red;
}

.option:hover img {
  padding: 2%;
  border: 5px solid lightblue;
  border-radius: 10px;
}

@media screen and (max-width: 786px) {
  h1 {
    font-size: 20px;
  }
  .option {
    background: rgb(34, 34, 32);
    padding: 4%;
    height: auto;
    position: relative;
    top: 10vh;
    text-align: center;
  }
  .option p {
    font-size: 10px;
    color: red;
  }
}
</style>
