<script setup></script>

<template>
  <header class="position-fixed w-100" :style="{ zIndex: '2000' }">
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark py-2">
      <div class="container">
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse d-flex justify-content-end" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <a class="nav-link text-white-50 text-center me-3" href="#abilities">專業技能</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-white-50 text-center me-3" href="#projects">專案作品</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-white-50 text-center me-3" href="#resume">自我介紹</a>
            </li>
            <li class="nav-item">
              <a class="nav-link text-white-50 text-center" href="#workExp">工作經歷</a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
  </header>
</template>
