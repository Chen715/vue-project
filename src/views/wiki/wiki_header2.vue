<template>
    <el-menu
      :default-active="activeIndex"
      class="el-menu-demo"
      mode="horizontal"
      :ellipsis="false"
      @select="handleSelect"
    >
      <el-menu-item index="0">
        <el-icon><Expand /></el-icon>
      </el-menu-item>
      
      <div class="flex-grow" />
      <el-menu-item index="1">
        <h1 style="font-size: 35px"> 1234 </h1>
      </el-menu-item>
    </el-menu>
  </template>
  
  <script lang="ts" setup>
  import { ref } from 'vue'
  import {
    Document,
    Menu as IconMenu,
    Location,
    Expand,
  } from '@element-plus/icons-vue'

  const activeIndex = ref('1')
  const handleSelect = (key: string, keyPath: string[]) => {
    console.log(key, keyPath)
  }
  </script>
  
  <style>

  /* 去掉边框白线 */
  .el-menu {
      border-right: 0;
    }

  </style>