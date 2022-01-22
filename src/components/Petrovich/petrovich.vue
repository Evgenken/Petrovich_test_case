<template>
  <div class="intro">
    <div class="logo">
      <div class="logo__item-1"><img src="@/assets/img/logo.png"> </div>
      <div class="logo__item-2"><img src="@/assets/img/SVGID.png"></div>
      </div>
          <div class="intro__text">лайфхаки и сервисы, которые пригодятся всем</div>
          <div class="circle-1"><img src="@/assets/img/Ellipse 8.png"></div>
    <div class="slogan">
      <div class="slogan__item-1"><img src="@/assets/img/Р.png"></div>
      <div class="slogan__item-1"><img src="@/assets/img/Е.png"></div>
      <div class="slogan__item-1"><img src="@/assets/img/М.png"></div>
      <div class="slogan__item-1"><img src="@/assets/img/О1.png"></div>
      <div class="slogan__item-1"><img src="@/assets/img/Н.png"></div>
      <div class="slogan__item-1"><img src="@/assets/img/Т1.png"></div>
    </div>
    <div class="img-slogan">
      <div class="img-slogan__instrument-1"><img src="@/assets/img/roulette.png"></div>
      <div class="img-slogan__instrument-2"><img src="@/assets/img/bucket.png"></div>
      <div class="stair"><img src="@/assets/img/stairs.png"></div>
  </div>
    <div class="slogan">
      <div class="slogan__item-2"><img src="@/assets/img/Б2.png"></div>
      <div class="slogan__item-2"><img src="@/assets/img/Е2.png"></div>
      <div class="slogan__item-2"><img src="@/assets/img/З1.png"></div>
      <div class="slogan__item-2"><img src="@/assets/img/З2.png"></div>
      <div class="slogan__item-2"><img src="@/assets/img/А.png"></div>
      <div class="slogan__item-2"><img src="@/assets/img/Б2.png"></div>
      <div class="slogan__item-2"><img src="@/assets/img/О2.png"></div>
      <div class="slogan__item-2"><img src="@/assets/img/Т2.png"></div>
    </div>
      <svg class="ellipse" height="6" width="80">
      <ellipse rx="40" ry="72" cx="3" cy="4"></ellipse>
      </svg>
  </div>
</template>

<script>

</script>

<style scoped lang="scss">

/* Intro */
.intro{
  height: 768px;
  width: 100%;
  background: #F8CB46;
}
.intro__text {
  font-family: "Graphik Cy";
  font-weight: bold;
  font-size: 32px;
  text-align: center;
  color: #DC3830;
  padding-top: 91px;
}
.logo {
  display: flex;
justify-content: space-between;
  align-items: center;
  padding-top: 20px;
  &__item-1{
    margin-left: 150px;
  }
  &__item-2{
    margin-right: 150px;
  }
}
.slogan{
  display: flex;
justify-content: center;
&__item-1{
  margin-left: 5px;
z-index: 1;
  padding-top: 20px;
}
  &__item-2{
    z-index: 1;
    margin-left: 15px;
    padding-top: 20px;
  }
}
.stair{
  position: absolute;
 justify-content: center;
  padding-right: 200px;
  padding-top: 250px;
  z-index: 2;
}
.ellipse{
justify-content: center;
  padding-left: 50%;
  padding-top: 100px;
  background: radial-gradient(circle at center,#F8CB46 100%,#F8CB46 0);
  z-index: 1;
}
/*img*/

.img-slogan {
  justify-content: center;
  display: flex;
  align-items: center;

  &__instrument-1 {
    position: absolute;
    margin-right: 500px;
    animation-duration: 3s;
    animation-name: roulette;
  }
  &__instrument-2{
    position: absolute;
    margin-left: 500px;
    animation-duration: 3s;
    animation-name: bucket;
  }
}
@keyframes roulette {
  from{
    margin-left: 10%;
width: 100%;
  }
  to{
    margin-right: 500px;
width: 18.3%;
  }
}
@keyframes bucket {
  from{
    margin-right: -150%;
    width: 100%;
  }
  to{
    margin-left: 500px;
    width: 12.1%;
  }
}
/* circle */

.circle-1{
  position: absolute;
  justify-content: center;
  padding-left: 250px;
}
</style>
