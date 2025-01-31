<template>
  <div class="container">
    <div class="row justify-content-center">
      <div class="modal-header" dir="rtl">
        <h5 class="modal-title py-5 px-5 fs-3 green-text fw-bolder">فوائد الألواح الشمسية ...</h5>
      </div>
      <div class="col-12 col-md-5 mb-3" v-for="(card, index) in cards" :key="index">
        <div class="card border-success w-100 h-100">
          <div class="d-flex justify-content-center align-items-center mt-4">
            <i :class="card.iconClass"></i>
          </div>
          <div class="card-body text-center">
            <h5 class="card-title fw-bolder fs-4">{{ card.title }}</h5>
            <p class="card-text">{{ card.description }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const cards = [
  {
    iconClass: 'bi bi-cash-coin icons',
    title: 'الطاقة كعملة',
    description: 'المعاملات التي تعمل بالطاقة المتجددة',
  },
  {
    iconClass: 'bi bi-lightning-charge-fill icons',
    title: 'مزود الطاقة الخضراء',
    description: 'تمكين الجميع من توريد الطاقة الخضراء وتداولها',
  },
  {
    iconClass: 'bi bi-arrows-fullscreen icons',
    title: 'إضفاء الطابع الديمقراطي على الوصول إلى مصادر الطاقة المتجددة',
    description: 'بسيط وسهل',
  },
  {
    iconClass: 'bi bi-graph-up-arrow icons',
    title: 'النمو',
    description: 'معاملات طاقة قابلة للتطوير لتنمية تدفقات إيرادات جديدة',
  },
]
</script>

<style scoped>
.green-text {
  color: rgb(32, 150, 32);
}
.icons {
  font-size: 2rem;
}
</style>
