<script setup>
const projectList = [
  {
    name: 'Black Heart 麵包電商網站',
    description:
      '使用 React 框架開發。電商購物車功能，透過串接API呈現產品資訊及活動訊息，並可透過後台系統隨時更改內容。',
    frontFunction: [
      '商品瀏覽：支援依產品分類及單一商品檢視',
      '購物車與結帳流程：優惠碼套入、訂單建立',
      '管理者帳號登入：管理者後台登入',
      'RWD 響應式設計：支援手機及電腦',
    ],
    backFunction: [
      '商品管理：新增、編輯商品內容',
      '訂單管理：查看訂單狀態並更改',
      '優惠券管理：新增及編輯優惠券',
      '活動資訊管理：新增或編輯活動資訊',
    ],
    imgUrl: 'bread.png',
    pageUrl: 'https://s870012.github.io/ReactFinal/',
    githubUrl: 'https://github.com/s870012/ReactFinal',
    tables: ['ReactJS', 'JavaScript', 'Bootstrap', 'AJAX'],
  },
  {
    name: '學識伴 LearnPlus++',
    description:
      '團隊共同開發，依據使用者 MBTI 屬性，推薦適合的課程或文章，使用者可依據教師 MBTI 屬性不同購買適合課程。',
    frontFunction: [
      '商品瀏覽：商品列表及示範商品瀏覽',
      'RWD 響應式設計：支援手機及電腦',
      '管理者帳號登入',
    ],
    backFunction: [],
    imgUrl: 'LearnPlus.png',
    pageUrl: 'https://hexschool2024d12.github.io/learnplus/index.html',
    githubUrl: 'https://github.com/hexschool2024d12/learnplus',
    tables: ['JavaScript', 'Bootstrap', 'SCSS'],
  },
]

const getImg = (img) => {
  return new URL(`../asset/images/${img}`, import.meta.url).href
}
</script>

<template>
  <section id="projects">
    <div class="container py-5">
      <h2 class="fw-bold mb-4">專案作品</h2>
      <div class="row mb-4">
        <div class="col-md-5">
          <img
            :src="getImg(projectList[0].imgUrl)"
            alt=""
            class="d-block w-100 rounded-2 border"
            :style="{ height: '350px' }"
          />
        </div>
        <div class="col-md-7 d-flex flex-column">
          <div class="mb-4">
            <h3 class="fw-bold mb-2">{{ projectList[0].name }}</h3>
            <p class="mb-2">
              {{ projectList[0].description }}
            </p>
            <ul class="d-flex list-unstyled mb-2 fs-7">
              <li
                class="bg-info text-white rounded-1 me-2 px-1"
                v-for="table in projectList[0].tables"
                :key="table"
              >
                {{ table }}
              </li>
            </ul>
          </div>
          <div class="d-flex">
            <div class="me-5">
              <h5 class="mb-2">前台功能：</h5>
              <ul>
                <li v-for="front in projectList[0].frontFunction" :key="front">{{ front }}</li>
              </ul>
            </div>
            <div>
              <h5 class="mb-2">後台功能：</h5>
              <ul>
                <li v-for="back in projectList[0].backFunction" :key="back">{{ back }}</li>
              </ul>
            </div>
          </div>
          <div class="d-flex justify-content-end mt-auto">
            <a :href="projectList[0].pageUrl" class="btn btn-outline-danger me-2" target="_blanket">
              網站連結 <i class="bi bi-box-arrow-right"></i>
            </a>
            <a :href="projectList[0].githubUrl" target="_blanket" class="btn btn-outline-danger"
              >GitHub <i class="bi bi-box-arrow-right"></i
            ></a>
          </div>
        </div>
      </div>
      <div class="row">
        <div class="col-md-5">
          <img
            :src="getImg(projectList[1].imgUrl)"
            alt=""
            class="d-block w-100 rounded-2 border"
            :style="{ height: '350px' }"
          />
        </div>
        <div class="col-md-7 d-flex flex-column">
          <div class="mb-4">
            <h3 class="fw-bold mb-2">{{ projectList[1].name }}</h3>
            <p class="mb-2">
              {{ projectList[1].description }}
            </p>
            <ul class="d-flex list-unstyled mb-2 fs-7">
              <li
                class="bg-info text-white rounded-1 me-2 px-1"
                v-for="table in projectList[1].tables"
                :key="table"
              >
                {{ table }}
              </li>
            </ul>
          </div>
          <div class="d-flex">
            <div class="me-5">
              <h5 class="mb-2">前台功能：</h5>
              <ul>
                <li v-for="front in projectList[1].frontFunction" :key="front">{{ front }}</li>
              </ul>
            </div>
          </div>
          <div class="d-flex justify-content-end mt-auto">
            <a :href="projectList[1].pageUrl" class="btn btn-outline-danger me-2" target="_blanket">
              網站連結 <i class="bi bi-box-arrow-right"></i>
            </a>
            <a :href="projectList[1].githubUrl" target="_blanket" class="btn btn-outline-danger"
              >GitHub <i class="bi bi-box-arrow-right"></i
            ></a>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.fs-7 {
  font-size: 12px;
}
</style>
