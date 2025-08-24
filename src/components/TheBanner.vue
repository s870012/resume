<script setup></script>

<template>
  <section>
    <div class="bg-banner">
      <div class="container pt-5 mb-5">
        <div class="row flex-column flex-md-row py-5">
          <div class="col-3">
            <img
              src="../asset/images/selfie.jpg"
              alt=""
              class="d-block border rounded-circle object-fit-cover"
              :style="{ height: '200px', width: '200px' }"
            />
          </div>
          <div class="col-9">
            <div class="d-lg-flex align-items-center justify-content-between">
              <div>
                <h1 class="fw-bold fs-64 mb-3">Name</h1>
                <p class="fs-3 mb-4">期望職位：前端工程師</p>
                <p class="text-black-50">
                  <em>
                    熟悉與客戶溝通需求，能以非技術語言清楚傳達並了解客戶的痛點。<br />擅長跨部門協作與資源整合，扮演中間橋樑角色，提升效率與專案開發速度。
                  </em>
                </p>
              </div>
              <div class="text-end">
                <p><i class="bi bi-envelope"></i> 連絡電話 : 0988-000000</p>
                <p><i class="bi bi-telephone"></i> 電子信箱 : eaxmple@gmail.com</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.fs-64 {
  font-size: 56px;
}
.bg-banner {
  background-image: url('../asset/images/Rectangle 3.png');
  background-position: right;
  background-size: contain;
  background-repeat: no-repeat;
}
</style>
