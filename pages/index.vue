<template>
  <div class="container">
    <div class="students-link">
      <h2>生徒一覧</h2>
      <nuxt-link to="/students" >生徒の情報を見る</nuxt-link>
    </div>
    <div class="managers-link">
      <h2>管理者一覧</h2>
      <nuxt-link to="/management" >管理者画面を見る</nuxt-link>
    </div>
  </div>
</template>

<style>
.container {
  justify-content: center;
  align-items: center;
  text-align: center;
  display: flex;
  min-height: 100vh;
}
.managers-link {
  margin-left: 30px;
}
</style>