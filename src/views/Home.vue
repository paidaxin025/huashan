<template>
  <div class="home">
    <el-container >
      <el-header>
        <v-header></v-header>
      </el-header>
      <el-container class="bott-container">
        <el-aside width="200px">
          <v-aside></v-aside>
        </el-aside>
        <el-main>Main</el-main>
      </el-container>
    </el-container>
  </div>
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header'
import Aside from '@/components/Aside'
export default {
  name: "Home",
  components: {
   'v-header': Header,
  'v-aside': Aside,
  },
};
</script>
<style scoped>
.bott-container {
  height: calc(100vh - 60px);
}
.el-header{
  padding: 0;
}
.el-aside {
  height: 100%;
  background-color: yellow;
}
.el-main {
  height: 100%;
  background-color: #eee;
}
</style>
