<template>
  <div>
    <div class="intro">
      <div class="logo">
        <div class="logo__item-1"><img src="@/assets/img/logo.png"> </div>
        <div class="logo__item-2"><img src="@/assets/img/SVGID.png"></div>
      </div>
      <div class="intro__text">лайфхаки и сервисы, которые пригодятся всем</div>
      <div class="img-slogan">
        <div class="img-slogan__circle-1"><img src="@/assets/img/Ellipse 8.png"></div>
        <div class="img-slogan__instrument-1"><img src="@/assets/img/roulette.png"></div>
        <div class="img-slogan__letters"><img src="@/assets/img/letters.png" alt=""></div>
        <div class="img-slogan__instrument-2"><img src="@/assets/img/bucket.png"></div>
      </div>
      <div class="img">
        <img src="@/assets/img/stair.png" class="img__stair">
      </div>
    </div>

      <div class="background">
        <img src="@/assets/img/background3.png" class="background__item-1">
        <div class="background__container"><img src="@/assets/img/Ellipse 15.png"></div>
      </div>
      <div class="rectangle"><img src="@/assets/img/Rectangle 1239.png"></div>

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

.img {
  width: 396px;
  height: 440px;
  position: absolute;
  overflow: hidden;
  bottom: 230px;
  left:calc(50% - 258px);
  z-index: 3;
   &__stair {
     animation-duration: 3s;
     animation-name: stair;
     position: relative;
   }
}

.background{
display: flex;
  position: relative;

 &__item-1{
max-width:100% ;
 }
  &__container{
    width: 44px;
    height: 87px;
    position: absolute;
    right: 0;
    bottom: -43px;
    overflow: hidden;
  }
}
/*img*/

.img-slogan {
  align-items: center;
  display: flex;
  justify-content: center;
  padding-top: 20px;

  &__circle-1{
    top: -170px;
    right: 30px;
    align-items: center;
    justify-content: center;
    position: relative;
  }

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
    margin-left: 600px;
    animation-duration: 3s;
    animation-name: bucket;
  }
}

@keyframes roulette {

  from{
    margin-right: 100%;
  }

  to{
    margin-right: 500px;
  }
}

@keyframes bucket {

  from{
    margin-left: 80%;
  }

  to{
    margin-left: 600;
  }
}

@keyframes stair {

  from{
    margin-top: 500px;
  }

  to{
    margin-top: 0;
  }
}

.rectangle{

  text-align: center;
  animation-name: rectangle;
  animation-duration: 1.5s;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
  animation-direction: alternate;
}
@keyframes rectangle {

  from{}

  to{
    margin-top: 30px;
  }
}

@media (max-width: 1280px) {

  .intro {
    height: 560px;

    &__text {
      font-size: 24px;
      padding-top: 70px;
    }
  }

  .logo {
    padding-top: 5px;

    &__item-1 {
      margin-left: 120px;
    }

    &__item-2 {
      margin-right: 120px;
    }
  }

  .img-slogan {
    transform: scale(69%);
    padding-top: 0px;
    margin-top: -50px;

    &__letters {
      transform: scale(0.85);
      padding-right: 50px;
    }

    &__circle-1 {
      top: -250px;
      right: -15px;
      transform: scale(131%);
    }

    &__instrument-1 {
      margin-left: -450px;
      z-index: 4;
    }

    &__instrument-2 {
      margin-right: -300px;
      transform: scale(121%);
    }
  }

  .img {
    transform: scale(80%);
    bottom: 350px;
  }

  .background__container {
    width: 87px;
    right: 40px;
    bottom: -43px;
  }
}

@media (max-width: 768px){

  .intro {
    height: 370px;

    &__text {
      font-size: 14px;
      padding-top: 50px;
      font-weight: normal;
    }
  }

  .logo {
    padding-top: 5px;
    transform: scale(0.8);
    &__item-1 {
      margin-left: -60px;
    }

    &__item-2 {
      margin-right: -60px;
    }
  }

  .img-slogan {
    transform: scale(35%);
    margin-top: -100px;

    &__letters {
      padding-right: 0;
    }

    &__circle-1 {
      display: none;
    }

    &__instrument-1 {
      bottom: -150px;
      left: -350px;
    }

    &__instrument-2 {
      bottom: -150px;
      right: -450px;
    }
  }

  .img {
    transform: scale(35%);
    top: 36px;
    left:calc(50% - 198px);
  }

  .background__container {
    transform: scale(0.5);
    right: -10px;
    bottom: 0;
  }
}

</style>
