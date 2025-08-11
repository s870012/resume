<script setup></script>

<template>
  <section>
    <div class="container py-5">
      <div class="row g-4">
        <h2 class="">專案作品</h2>
        <div class="col-4">
          <div class="card d-flex flex-column h-100">
            <div class="card-head">
              <img
                src="../asset/images/bread.png"
                alt=""
                class="d-block w-100 rounded-2"
                :style="{ height: '220px' }"
              />
            </div>
            <div class="card-body d-flex flex-column">
              <h5 class="mb-2">Black Heart麵包電商網站</h5>
              <ul class="d-flex list-unstyled mb-2 fs-7">
                <li class="bg-info text-white rounded-1 me-2 px-1">ReactJS</li>
                <li class="bg-info text-white rounded-1 me-2 px-1">JavaScript</li>
                <li class="bg-info text-white rounded-1 me-2 px-1">Bootstrap</li>
              </ul>
              <p class="mb-3">
                文青風的麵包電商網站，使用React框架開發。有基本的電商購物車功能，透過串接API呈現產品資訊及活動訊息，並可透過後台系統隨時更改內容。
              </p>
              <div class="d-flex mt-auto">
                <button type="button" class="btn btn-outline-danger me-2">
                  網站連結 <i class="bi bi-box-arrow-right"></i>
                </button>
                <button type="button" class="btn btn-outline-danger">
                  GitHub <i class="bi bi-box-arrow-right"></i>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="col-4">
          <div class="card d-flex flex-column h-100">
            <div class="card-head">
              <img
                src="../asset/images/LearnPlus.png"
                alt=""
                class="d-block w-100 rounded-2"
                :style="{ height: '220px' }"
              />
            </div>
            <div class="card-body d-flex flex-column">
              <h5 class="mb-2">學識伴LearnPlus++</h5>
              <ul class="d-flex list-unstyled mb-2 fs-7">
                <li class="bg-info text-white rounded-1 me-2 px-1">JavaScript</li>
                <li class="bg-info text-white rounded-1 me-2 px-1">Bootstrap</li>
                <li class="bg-info text-white rounded-1 me-2 px-1">SCSS</li>
              </ul>
              <p class="mb-3">
                團隊共同開發，依據使用者MBTI屬性，推薦適合的課程或文章，使用者可依據教師MBTI屬性不同購買適合課程。
              </p>
              <div class="d-flex mt-auto">
                <button type="button" class="btn btn-outline-danger me-2">
                  網站連結 <i class="bi bi-box-arrow-right"></i>
                </button>
                <button type="button" class="btn btn-outline-danger">
                  GitHub <i class="bi bi-box-arrow-right"></i>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="col-4">
          <div class="card d-flex flex-column h-100">
            <div class="card-head">
              <img
                src="../asset/images/bed.png"
                alt=""
                class="d-block w-100 rounded-2"
                :style="{ height: '220px' }"
              />
            </div>
            <div class="card-body d-flex flex-column">
              <h5 class="mb-2">SPA電商網站</h5>
              <ul class="d-flex list-unstyled mb-2 fs-7">
                <li class="bg-info text-white rounded-1 me-2 px-1">JavaScript</li>
                <li class="bg-info text-white rounded-1 me-2 px-1">Bootstrap</li>
              </ul>
              <p>一頁式電商網站，選擇最適合的寢室家具。</p>
              <div class="d-flex mt-auto">
                <button type="button" class="btn btn-outline-danger me-2">
                  網站連結 <i class="bi bi-box-arrow-right"></i>
                </button>
                <button type="button" class="btn btn-outline-danger">
                  GitHub <i class="bi bi-box-arrow-right"></i>
                </button>
              </div>
            </div>
          </div>
        </div>
        <div class="col-4">
          <div class="card d-flex flex-column h-100">
            <div class="card-head">
              <img
                src="../asset/images/travel.png"
                alt=""
                class="d-block w-100 rounded-2"
                :style="{ height: '220px' }"
              />
            </div>
            <div class="card-body d-flex flex-column">
              <h5 class="mb-2">旅遊網站</h5>
              <ul class="d-flex list-unstyled mb-2 fs-7">
                <li class="bg-info text-white rounded-1 me-2 px-1">Bootstrap</li>
                <li class="bg-info text-white rounded-1 me-2 px-1">SCSS</li>
                <li class="bg-info text-white rounded-1 me-2 px-1">vite</li>
              </ul>
              <p class="mb-3">旅遊網站製作，Bootstrap切版及RWD響應式設計。</p>
              <div class="d-flex mt-auto">
                <button type="button" class="btn btn-outline-danger me-2">
                  網站連結 <i class="bi bi-box-arrow-right"></i>
                </button>
                <button type="button" class="btn btn-outline-danger">
                  GitHub <i class="bi bi-box-arrow-right"></i>
                </button>
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
