<template>
  <div class="student_id">
  <session>
    <h1>{{ $route.params.id }}</h1>
  </session>
   <nuxt-link to="/index">生徒一覧へ戻る</nuxt-link>
    <nuxt-link to="/">トップページへ戻る</nuxt-link>
  </div>
</template>


<script>
export default {
  validate({ params }) {
  },
  data() {
    return {
      students: [
        {
          id: "qnfungqxllc3m1ak",
          name: "生徒A",
        },
        {
          id: "7j9cumkgsq6l264c",
          name: "生徒B",
        },
        { id: "eo34bhey9m0d92ou",
          name: "生徒C",
        },
      ],
    };
  }
};
</script>


<style>
.student_id {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
</style>