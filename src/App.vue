<script setup>
import TheAbilities from './components/TheAbilities.vue'
import TheProjects from './components/TheProjects.vue'
import WorkExp from './components/WorkExp.vue'
import TheResume from './components/TheResume.vue'
</script>

<template>
  <section>
    <div class="container">
      <div class="row py-5">
        <div class="col-9">
          <div class="d-flex align-items-center">
            <h1 class="fs-64 me-5">陳昭維</h1>
            <p class="fs-3">期望職位：前端工程師</p>
          </div>
          <p>電話 : 0988-189159</p>
          <p>電子信箱 : s8700122000@gmail.com</p>
        </div>
        <div class="col-3">
          <img
            src="./asset/images/selfie.jpg"
            alt=""
            class="d-block border rounded-circle object-fit"
            :style="{ height: '200px', width: '200px' }"
          />
        </div>
      </div>
    </div>
  </section>
  <TheAbilities />
  <TheProjects />
  <TheResume />
  <WorkExp />
</template>

<style scoped>
.fs-64 {
  font-size: 56px;
}
</style>
