<template>
  <div class="students">
    <div class="students-item">
      <h1>生徒一覧</h1>
        <ul>
            <li v-for="student in students" :key="student">
              <nuxt-link to="{path:'students/_id'}" >{{ student.name }}</nuxt-link>
            </li>
        </ul>
      <nuxt-link to="/" >戻る</nuxt-link>
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
.students {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  min-height: 100vh;
}
ul {
padding-left: 0;
}
li {
list-style: none;
}
</style>
