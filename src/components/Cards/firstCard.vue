<template>
  <div class="card flex flex-row items-center card text-bg-success rounded-4">
    <div class="card-body flex flex-row justify-between w-full">
      <div class="flex-1 flex flex-col gap-5">
        <h2 class="card-title fw-bold fs-1 pt-5 ps-5">We transform energy into currency</h2>
        <p class="card-text fs-4 lh-lg pt-2 pe-5 ps-5">
          backbone.one converts every energy transaction into monetary value. We are dedicated to
          democratizing access to renewable energy and laying the groundwork for innovative business
          models in the Internet of Energy.
        </p>
      </div>
      <div class="flex-1 text-right pt-4 ps-5">
        <a href="#" class="btn btn-light btn-lg btn-outline-success rounded-pill">Go somewhere</a>
      </div>
    </div>

    <div class="card-body flex-1">
      <div class="background">
        <div class="cardWrapper">
          <div class="rotate">
            <div class="front">
              <img src="https://100dayscss.com/codepen/bycicle.svg" class="image" />
              <div class="roadWrapper">
                <div class="line-1"></div>
                <div class="line-2"></div>
                <div class="line-3"></div>
                <div class="line-4"></div>
                <div class="line-5"></div>
                <div class="line-6"></div>
                <div class="line-7"></div>
              </div>
            </div>
            <div class="back">
              <img src="https://100dayscss.com/codepen/helicopter.svg" class="image" />
              <div class="skyWrapper">
                <div class="cloud-1"></div>
                <div class="cloud-2"></div>
                <div class="cloud-3"></div>
                <div class="cloud-4"></div>
                <div class="cloud-5"></div>
                <div class="cloud-6"></div>
                <div class="cloud-7"></div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="js" setup></script>

<style scoped>
@import url(https://fonts.googleapis.com/css?family=Open+Sans:700,600,500,400);

body {
  margin: 0;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  font-family: 'Open Sans', 'Lucida Sans Unicode', 'Lucida Grande', sans-serif;
  font-size: 14px;
}

.background {
  position: relative;
  background: linear-gradient(to bottom, #222 100%);
  width: 400px;
  height: 400px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.cardWrapper {
  display: flex;
  flex-direction: column;
  width: 320px;
  height: 200px;
  perspective: 500px;
}

.cardWrapper:hover .rotate {
  transform: rotateX(180deg) translate3d(0, 0, 0);
  box-shadow: 8px -10px 15px 0 rgba(0, 0, 0, 0.5);
}

.rotate {
  position: relative;
  width: 100%;
  height: 100%;
  transform-style: preserve-3d;
  transition: all 1s ease-in-out;
  perspective: 1000px;
  box-shadow: 8px 10px 15px 0 rgba(0, 0, 0, 0.5);
}

.front,
.back {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 100%;
  background: #80b58f;
  backface-visibility: hidden;
  border-radius: 3px;
  overflow: hidden;
  text-align: center;
}

.front {
  z-index: 2;
  transform: rotateX(0);
}

.back {
  z-index: 1;
  transform: rotateX(180deg);
}

.image {
  position: relative;
  transform-origin: 50% 100%;
}

.roadWrapper {
  position: absolute;
  top: 133px;
  left: 80px;
  width: 200px;
  height: 3px;
  overflow: hidden;
}

.roadWrapper .line-1,
.roadWrapper .line-2,
.roadWrapper .line-3,
.roadWrapper .line-4,
.roadWrapper .line-5,
.roadWrapper .line-6,
.roadWrapper .line-7 {
  position: absolute;
  right: -25px;
  top: 0;
  height: 3px;
  background: #fffefd;
  border-radius: 3px;
}

.roadWrapper .line-1 {
  width: 4px;
  animation: lines 0.8s linear infinite;
}

.roadWrapper .line-2 {
  width: 6px;
  animation: lines 0.9s linear infinite;
}

.roadWrapper .line-3 {
  width: 8px;
  animation: lines 1s linear infinite;
}

.roadWrapper .line-4 {
  width: 10px;
  animation: lines 1.1s linear infinite;
}

.roadWrapper .line-5 {
  width: 12px;
  animation: lines 1.2s linear infinite;
}

.roadWrapper .line-6 {
  width: 14px;
  animation: lines 1.3s linear infinite;
}

.roadWrapper .line-7 {
  width: 16px;
  animation: lines 1.4s linear infinite;
}

.skyWrapper {
  position: absolute;
  top: 23px;
  bottom: 0;
  left: 80px;
  width: 200px;
  height: 150px;
  overflow: hidden;
}

.skyWrapper .cloud-1,
.skyWrapper .cloud-2,
.skyWrapper .cloud-3,
.skyWrapper .cloud-4,
.skyWrapper .cloud-5,
.skyWrapper .cloud-6,
.skyWrapper .cloud-7 {
  position: absolute;
  right: -25px;
  height: 3px;
  background: #eaecee;
  border-radius: 3px;
}

.skyWrapper .cloud-1 {
  top: 20px;
  width: 20px;
  animation: lines 0.6s linear infinite;
}

.skyWrapper .cloud-2 {
  top: 34px;
  width: 24px;
  animation: lines 0.7s linear infinite;
}

.skyWrapper .cloud-3 {
  top: 48px;
  width: 28px;
  animation: lines 0.8s linear infinite;
}

.skyWrapper .cloud-4 {
  top: 62px;
  width: 32px;
  animation: lines 0.9s linear infinite;
}

.skyWrapper .cloud-5 {
  top: 76px;
  width: 36px;
  animation: lines 1s linear infinite;
}

.skyWrapper .cloud-6 {
  top: 90px;
  width: 40px;
  animation: lines 1.1s linear infinite;
}

.skyWrapper .cloud-7 {
  top: 104px;
  width: 44px;
  animation: lines 1.2s linear infinite;
}

@keyframes ride {
  0%,
  100% {
    transform: scaleY(1);
  }
  50% {
    transform: scaleY(0.96);
  }
}

@keyframes fly {
  0%,
  100% {
    transform: translate3d(0, -10px, 0);
  }
  50% {
    transform: translate3d(0, 10px, 0);
  }
}

@keyframes lines {
  0% {
    transform: translate3d(0, 0, 0);
  }
  100% {
    transform: translate3d(-250px, 0, 0);
  }
}
</style>
