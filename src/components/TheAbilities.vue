<script setup>
const abilityList = [
  {
    id: 'a001',
    name: 'React、Vue',
    imgUrl: ['react-icon.png', 'vue-icon.png'],
    contents: [
      '使用Vite開發SPA電商網站',
      '模組化開發-使用Components實作',
      '前後端分離開發',
      'Router應用',
      'Redux Toolkit應用',
    ],
  },
  {
    id: 'a002',
    name: 'JavaScript',
    imgUrl: ['js-icon.png'],
    contents: [
      '熟悉AJAX / JSON格式與串接API<',
      '模組化開發-熟悉ES6標準與JavaScript特性(this、一級涵式、高階函式應用)',
    ],
  },
  {
    id: 'a003',
    name: 'Web Layout',
    imgUrl: ['css-icon.png'],
    contents: [
      'HTML5、CSS',
      '使用SCSS開發，熟悉Smacss與OOCSS開發模式',
      '模組化開發-熟悉Bootstrap 5及客製化、RWD自適應網頁開發',
    ],
  },
  {
    id: 'a004',
    name: 'Others',
    imgUrl: ['other-icon.png'],
    contents: ['Git、GitHub', '模組化開發-理解Git Flow工作流程'],
  },
]

const getImg = (img) => {
  return new URL(`../asset/images/${img}`, import.meta.url).href
}
</script>

<template>
  <section class="py-5 bg-light" id="abilities">
    <div class="container">
      <div class="row">
        <h2 class="fw-bold mb-3">專業技能</h2>
        <div class="col-sm-6 col-md-3" v-for="ability in abilityList" :key="ability.id">
          <div class="card border-0 bg-light">
            <div class="d-flex align-items-center">
              <img
                v-for="img in ability.imgUrl"
                :key="img"
                :src="getImg(img)"
                alt="icon"
                class="d-block me-1"
                :style="{ height: '40px', maxWidth: '100' }"
              />
              <h4 class="card-head">{{ ability.name }}</h4>
            </div>
            <div class="card-body">
              <ul class="list-unstyled">
                <li v-for="item in ability.contents" :key="item" class="mb-2">{{ item }}</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
