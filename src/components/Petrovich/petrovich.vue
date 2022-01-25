<template>
  <div class="intro">
    <div class="intro__background"><img src="@/assets/img/background.png"></div>
    <div class="logo">
      <div class="logo__item-1"><img src="@/assets/img/logo.png"> </div>
      <div class="logo__item-2"><img src="@/assets/img/SVGID.png"></div>
      </div>
          <div class="intro__text">лайфхаки и сервисы, которые пригодятся всем</div>
          <div class="circle-1"><img src="@/assets/img/Ellipse 8.png"></div>
    <div class="img-slogan">
      <div class="img-slogan__instrument-1"><img src="@/assets/img/roulette.png"></div>
      <div class="img-slogan__letters"><img src="@/assets/img/letters.png" alt=""></div>
      <div class="img-slogan__instrument-2"><img src="@/assets/img/bucket.png"></div>
  </div>
    <div class="stair"><img src="@/assets/img/stair.png"></div>
  </div>
</template>

<script>

</script>

<style scoped lang="scss">

/* Intro */
.intro{
  height: 768px;
  width: 100%;
  overflow: hidden;
}
.intro__text {
  font-family: "Graphik Cy", sans-serif;
  font-weight: bold;
  font-size: 32px;
  text-align: center;
  color: #DC3830;
  padding-top: 91px;
  position: relative;
}
.intro__background{
  position: absolute;
}
.logo {
  display: flex;
justify-content: space-between;
  align-items: center;
  padding-top: 20px;
  &__item-1{
    margin-left: 150px;
    z-index: 1;
  }
  &__item-2{
    margin-right: 150px;
    z-index: 1;
  }
}

.stair{
  position: relative;
  text-align: center;
  padding-right: 200px;
  z-index: 2;
  animation-duration: 3s;
  animation-name: stair;
}
/*img*/

.img-slogan {
  align-items: center;
  display: flex;
  justify-content: center;
  padding-top: 20px;
  box-sizing: border-box;
  &__letters{
    z-index: 3;
  }
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
@keyframes stair {
  from{
    margin-top: -150%;
    height: 100%;
  }
  to{
    margin-top: 500px;
    height: 12.1%;
  }
}
/* circle */

.circle-1{
  position: absolute;
  justify-content: center;
  padding-left: 250px;
}
</style>
