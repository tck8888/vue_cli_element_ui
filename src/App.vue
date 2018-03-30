<template>
  <div id="app">
  <el-container style="height: 100%; border: 1px solid #eee">
        <el-aside width="200px" style="background-color: rgb(238, 241, 246)">
           <el-menu :default-active="$route.path" router>
              <el-submenu index="1">
                <template slot="title"><i class="el-icon-message"></i>操作系统</template>
                <el-menu-item-group>
                  <template slot="title">单选题</template>
                  <el-menu-item index="/">第一题</el-menu-item>
                  <el-menu-item index="/hi">第二题</el-menu-item>
                </el-menu-item-group>
                 <el-menu-item-group>
                  <template slot="title">多选题</template>
                  <el-menu-item index="1-3">第三题</el-menu-item>
                </el-menu-item-group>
              </el-submenu>
           </el-menu>
        </el-aside>
        <el-main><router-view/></el-main>
    </el-container>
  </div>
</template>

<script>
export default {
  name: "App"
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
