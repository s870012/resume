<script setup>
const imgList = [
  {
    id: 1,
    imgUrl: 'React-finish.png',
    description: 'React 作品實戰班 - 2024 冬季班',
  },
  {
    id: 2,
    imgUrl: 'test-award.png',
    description: '2024 網頁切版專題班 上機考證書',
  },
]

const getImg = (img) => {
  return new URL(`../asset/images/${img}`, import.meta.url).href
}
</script>

<template>
  <section id="resume" class="bg-gray">
    <div class="container py-5">
      <div class="row">
        <div class="col-10 mx-auto">
          <div class="text-align blockquote">
            <h2 class="fw-bold mb-3">自我介紹</h2>
            <div class="lh-lg mb-3">
              <h5 class="fw-bold">學歷：</h5>
              <div class="d-flex justify-content-between align-items-center">
                <p>國立臺灣海洋大學 運輸科學系碩士</p>
                <p class="text-black-50 fs-6">2014.09 - 2016.07</p>
              </div>
            </div>
            <div class="lh-lg mb-3">
              <h5 class="fw-bold">個人特質：</h5>
              <p>
                個性溫和、具親和力，擅長溝通與協調，能與同儕及同事維持良好互動，營造和諧工作氛圍。
              </p>
            </div>
            <div class="lh-lg mb-3">
              <h5 class="fw-bold">學習態度：</h5>
              <p>
                樂於學習並不斷自我成長，積極學習前端知識拓展跨領域能力，始終保持對學習的渴望，相信「投資自己」是最有價值的選擇。
              </p>
            </div>
            <div class="lh-lg">
              <h5 class="fw-bold">前端之路：</h5>
              <p>
                參加六角學院的「前端 React
                培訓班」。這門課程涵蓋了完整且紮實的前端基礎知識，讓我決定毅然決然地投入學習。<strong>
                  經過為期 9 個月的密集訓練</strong
                >，我系統性地掌握了網頁切版、JavaScript 程式語言以及 React
                框架的核心概念與實作能力。學習期間，我完成一個React實戰作品、三個切版作品，也參與團隊合作開發專案，從需求溝通、UI
                規劃到功能開發與問題排解，完整體驗了實際開發流程，為未來職場銜接打下了穩固的基礎。這段學習歷程不僅強化了我的技術能力，也讓我對於成為一名前端工程師充滿信心。
              </p>
            </div>
          </div>
        </div>
      </div>
      <div class="row g-4">
        <div class="col-10 mx-auto">
          <h4 class="fw-bold text-center">課程證書</h4>
        </div>
        <div class="col-sm-6" v-for="img in imgList" :key="img.id">
          <img :src="getImg(img.imgUrl)" alt="certificate" class="d-block w-100 mb-1 rounded-1" />
          <p class="text-center">{{ img.description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.text-align {
  text-align: justify;
}
.bg-gray {
  background-color: #f0f0f0;
}
</style>
