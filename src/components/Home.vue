<template>
  <div>
   <el-row class="tac">
   <el-col :span="4">
    <el-menu
      default-active="2"
      class="el-menu-vertical-demo"
      @open="handleOpen"
      @close="handleClose"
      background-color="#545c64"
      text-color="#fff"
      active-text-color="#ffd04b">
      <el-submenu index="1">
        <template slot="title">
          <i class="el-icon-s-platform"></i>
          <span>菜单一</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="1-1">菜单1</el-menu-item>
          <el-menu-item index="1-2">菜单1</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
       <el-submenu index="2">
        <template slot="title">
          <i class="el-icon-s-tools"></i>
          <span>系统设置</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="1-1">权限管理</el-menu-item>
          <el-menu-item index="1-2">角色管理</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-submenu index="3">
        <template slot="title">
          <i class="el-icon-user-solid"></i>
          <span>用户管理</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="1-1">人员1</el-menu-item>
          <el-menu-item index="1-2">人员2</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
      <el-submenu index="4">
        <template slot="title">
          <i class="el-icon-message-solid"></i>
          <span>菜单1</span>
        </template>
        <el-menu-item-group>
          <el-menu-item index="1-1">菜单1</el-menu-item>
          <el-menu-item index="1-2">菜单1</el-menu-item>
        </el-menu-item-group>
      </el-submenu>
    </el-menu>
  </el-col>
</el-row>
  </div>
</template>
<script>
export default {
  methods: {
    handleOpen (key, keyPath) {
      console.log(key, keyPath)
    },
    handleClose (key, keyPath) {
      console.log(key, keyPath)
    }
  }
}
</script>
