<script lang="ts">
export default {
  name: 'Person',
  data() {
    return {
      name: 'Max',
      age: 30,
      Tel: '1234567890'
    }
  },
  methods: {
    showTel() {
      alert(this.Tel)
    },
    changeName() {
      this.name = 'Min'
    },
    changeAge() {
      this.age = 20
    }
  }
}
</script>

<template>
  <div class="Person">
    <h2>姓名：{{ name }}</h2>
    <h2>年龄：{{ age }}</h2>
    <button @click="changeName">修改名字</button>
    <button @click="changeAge">修改年龄</button>
    <button @click="showTel">查看联系方式</button>

  </div>
</template>

<style scoped>
.Person {
  background-color: skyblue;
  box-shadow: 0 0 10px;
  border-radius: 10px;
  padding: 20px;
}
</style>