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
      <div class="row g-4">
        <h2 class="fw-bold">專案作品</h2>
        <div class="col-sm-6" v-for="project in projectList" :key="project">
          <div class="card d-flex flex-column h-100">
            <div class="card-head">
              <img
                :src="getImg(project.imgUrl)"
                alt=""
                class="d-block w-100 rounded-2"
                :style="{ height: '350px' }"
              />
            </div>
            <div class="card-body d-flex flex-column">
              <h5 class="mb-2">{{ project.name }}</h5>
              <ul class="d-flex list-unstyled mb-2 fs-7">
                <li
                  class="bg-info text-white rounded-1 me-2 px-1"
                  v-for="table in project.tables"
                  :key="table"
                >
                  {{ table }}
                </li>
              </ul>
              <p class="mb-3">
                {{ project.description }}
              </p>
              <ul>
                <li v-for="content in project.frontFunction" :key="content">{{ content }}</li>
              </ul>
              <div class="d-flex mt-auto">
                <a :href="project.pageUrl" class="btn btn-outline-danger me-2" target="_blanket">
                  網站連結 <i class="bi bi-box-arrow-right"></i>
                </a>
                <a :href="project.githubUrl" target="_blanket" class="btn btn-outline-danger"
                  >GitHub <i class="bi bi-box-arrow-right"></i
                ></a>
              </div>
            </div>
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
