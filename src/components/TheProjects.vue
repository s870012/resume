<script setup>
const projectList = [
  {
    name: 'Black Heart麵包電商網站',
    description:
      '文青風的麵包電商網站，使用React框架開發。有基本的電商購物車功能，透過串接API呈現產品資訊及活動訊息，並可透過後台系統隨時更改內容。',
    imgUrl: 'bread.png',
    pageUrl: 'https://s870012.github.io/ReactFinal/',
    githubUrl: 'https://github.com/s870012/ReactFinal',
    tables: ['ReactJS', 'JavaScript', 'Bootstrap', 'AJAX'],
  },
  {
    name: '學識伴LearnPlus++',
    description:
      '團隊共同開發，依據使用者MBTI屬性，推薦適合的課程或文章，使用者可依據教師MBTI屬性不同購買適合課程。',
    imgUrl: 'LearnPlus.png',
    pageUrl: 'https://hexschool2024d12.github.io/learnplus/index.html',
    githubUrl: 'https://github.com/hexschool2024d12/learnplus',
    tables: ['JavaScript', 'Bootstrap', 'SCSS'],
  },
  {
    name: '一頁式電商網站',
    description: '一頁式電商網站，選擇最適合的寢室家具。',
    imgUrl: 'bed.png',
    pageUrl: 'https://s870012.github.io/JSFinal/index.html',
    githubUrl: 'https://github.com/s870012/JSFinal/tree/main',
    tables: ['JavaScript', 'Bootstrap'],
  },
  {
    name: '旅遊網站',
    description: '旅遊網站製作，Bootstrap切版及RWD響應式設計。',
    imgUrl: 'travel.png',
    pageUrl: 'https://s870012.github.io/layoutweek6/index.html',
    githubUrl: 'https://github.com/s870012/layoutweek6',
    tables: ['Bootstrap', 'SCSS', 'vite'],
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
        <div class="col-4" v-for="project in projectList" :key="project">
          <div class="card d-flex flex-column h-100">
            <div class="card-head">
              <img
                :src="getImg(project.imgUrl)"
                alt=""
                class="d-block w-100 rounded-2"
                :style="{ height: '220px' }"
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
