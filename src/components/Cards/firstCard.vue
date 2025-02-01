<template>
  <div class="card d-flex flex-column flex-md-row align-items-center text-bg-success rounded-4 p-4">
    <!-- Animation Section -->
    <div class="card-body col-12 col-md-6 d-flex justify-content-center">
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

    <!-- Text Content Section -->
    <div class="card-body col-12 col-md-6 d-flex flex-column justify-content-between p-4">
      <div>
        <h2 class="card-title fw-bold fs-1 text-md-end text-center">
          نحول الطاقة إلى عملة
        </h2>
        <p class="card-text fs-4 lh-lg text-md-end text-center">
          يحول كل معاملة طاقة إلى قيمة نقدية. نحن ملتزمون بإضفاء الطابع الديمقراطي على الوصول إلى
          الطاقة المتجددة وإرساء الأساس للأعمال المبتكرة نماذج في إنترنت الطاقة.
        </p>
      </div>
      <div class="text-md-end text-center">
        <a href="#" class="btn btn-outline-light btn-lg rounded-pill">المزيد</a>
      </div>
    </div>
  </div>
</template>

<script lang="js" setup></script>

<style scoped>
@import url(https://fonts.googleapis.com/css?family=Open+Sans:700,600,500,400);



.background {
  width: 100%;
  max-width: 400px;
  height: auto;
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
