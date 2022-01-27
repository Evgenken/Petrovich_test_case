<template>
  <div>
  <div class="intro">
    <div class="logo">
      <div class="logo__item-1"><img src="@/assets/img/logo.png"> </div>
      <div class="logo__item-2"><img src="@/assets/img/SVGID.png"></div>
      </div>
          <div class="intro__text">лайфхаки и сервисы, которые пригодятся всем</div>
    <div class="img-slogan">
      <div class="circle-1"><img src="@/assets/img/Ellipse 8.png"></div>
      <div class="img-slogan__instrument-1"><img src="@/assets/img/roulette.png"></div>
      <div class="img-slogan__letters"><img src="@/assets/img/letters.png" alt=""></div>
      <div class="img-slogan__instrument-2"><img src="@/assets/img/bucket.png"></div>
  </div>
    <div class="stair"><img src="@/assets/img/stair.png"></div>
  </div>
  <div>
    <div class="background">
      <img src="@/assets/img/background3.png" class="background_item-1">
      <img src="@/assets/img/Rectangle 1239.png" class="background__item-2">
      <img src="@/assets/img/Ellipse 15.png" class="background__item-3">
    </div>

  </div>
  </div>
</template>

<script>

</script>

<style scoped lang="scss">
*{
  box-sizing: border-box;
  padding: 0;
  margin: 0;
}
/* Intro */
.intro{
  height: 690px;
  width: 100%;
  overflow: hidden;
  display: flex;
  flex-direction:column;
  background: #F8CB46;
  flex: 1 0 auto;
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
  z-index: 3;
  animation-duration: 3s;
  animation-name: stair;
  position: absolute;
  bottom: 145px;
  left: 500px;
}
.background{

 &__item-1{
width-max:100% ;
 }
}
/*img*/

.img-slogan {
  align-items: center;
  display: flex;
  justify-content: center;
  padding-top: 20px;
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
    margin-top: -800px;
    height: 12.1%;
  }
}
/* circle */

.circle-1{

}
</style>
