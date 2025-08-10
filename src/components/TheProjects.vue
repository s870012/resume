<script setup></script>

<template>
  <section>
    <div class="container">
      <div class="row g-4">
        <h2 class="mb-3">專案作品</h2>
        <div class="col">
          <div class="card d-flex flex-column h-100">
            <div class="card-head">
              <img
                src="../asset/images/bread.png"
                alt=""
                class="d-block w-100"
                :style="{ height: '250px' }"
              />
            </div>
            <div class="card-body">
              <h4>Black Heart麵包電商網站</h4>
              <p>開發期間：2025/1-2025/4</p>
              <p>
                專案描述：文青風的麵包電商網站，使用Vite作為開發工具，並使用React框架開發。有基本的電商購物車功能，透過串接API呈現產品資訊及活動訊息，並可透過後台系統隨時更改內容。
              </p>
              <ul>
                <li></li>
                <li></li>
                <li></li>
              </ul>
              <div class="d-flex">
                <p class="p-2 me-2 border rounded-2 bg-light">
                  <a href="" class="text-decoration-none">網站連結 </a
                  ><i class="bi bi-1-circle-fill"></i>
                </p>
                <p class="p-2 border rounded-2">
                  <a href="" class="text-decoration-none">GitHub</a>
                </p>
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
                class="d-block w-100"
                :style="{ height: '250px' }"
              />
            </div>
            <div class="card-body">
              <h4>學識伴LearnPlus++</h4>
              <p>開發期間：2024/7-2024/10</p>
              <p>
                專案描述：與學員間共同發想製作，設計依據使用者MBTI屬性，推薦適合的課程或文章，使用者也能知道課堂教師MBTI屬性，作為購買課程的參考依據，並設計不同活動累積積分以吸引使用者。
              </p>
            </div>
          </div>
        </div>
        <div class="col-4">
          <div class="card d-flex flex-column h-100">
            <div class="card-head">
              <img
                src="../asset/images/bed.png"
                alt=""
                class="d-block w-100"
                :style="{ height: '250px' }"
              />
            </div>
            <div class="card-body">
              <h4>SPA電商網站</h4>
              <p>開發期間：2024/12-2025/1</p>
              <p>專案描述：一頁式電商網站，選擇最適合的寢室家具。</p>
            </div>
          </div>
        </div>
        <div class="col-4">
          <div class="card d-flex flex-column h-100">
            <div class="card-head">
              <img
                src="../asset/images/travel.png"
                alt=""
                class="d-block w-100"
                :style="{ height: '250px' }"
              />
            </div>
            <div class="card-body">
              <h4>旅遊網站</h4>
              <p>開發期間：2024/7-2024/7</p>
              <p>專案描述：旅遊網站製作，Bootstrap切版及RWD響應式設計。</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
