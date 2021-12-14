<template>
  <div class="management">
    <div class="manegement-item">
    <h1>生徒管理ページ</h1>
      <table>
        <tr>
        <th>名前</th>
        <th>ID</th>
        </tr>
        <tr　v-for="student in students" :key="student">
        <td>{{ student.name }}</td>
        <td>{{ student.id }}</td>
        </tr>
      </table>
      <nuxt-link to="/">戻る</nuxt-link>
    </div>
  </div>
</template>


<script>
export default {
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
        {
          id: "eo34bhey9m0d92ou",
          name: "生徒C",
        },
      ],
    };
  },
};
</script>


<style>
.management {
  display: flex;
  margin: 0 auto;
  min-height: 100vh;
  justify-content: center;
  align-items: center;
  text-align: center;
}
table {
   margin: 0 auto;
}
</style>
