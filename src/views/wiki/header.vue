<template>
    <el-menu
      :default-active="activeIndex"
      class="el-menu-demo"
      mode="horizontal"
      :ellipsis="false"
      @select="handleSelect"
    >
      <el-menu-item index="0">
        <h1 style="font-size: 35px"> 1234 </h1>
      </el-menu-item>
      
      <div class="flex-grow" />
      <el-menu-item index="1">Processing Center</el-menu-item>
        <el-sub-menu index="2" >
            <template #title >
               <h1> Workspace </h1> 
            </template>
            <el-menu-item index="2-1"><h1>item one</h1></el-menu-item>
            <el-menu-item index="2-2"><h1>item two</h1></el-menu-item>
            <el-menu-item index="2-3"><h1>item three</h1></el-menu-item>
            <el-sub-menu index="2-4">
                <template #title><h1>item four</h1></template>
                <el-menu-item index="2-4-1">item one</el-menu-item>
                <el-menu-item index="2-4-2">item two</el-menu-item>
                <el-menu-item index="2-4-3">item three</el-menu-item>
            </el-sub-menu>
        </el-sub-menu>

        
        <el-backtop :bottom="100">
          <div
            style="
              height: 100%;
              width: 100%;
              background-color: var(--el-bg-color-overlay);
              box-shadow: var(--el-box-shadow-lighter);
              text-align: center;
              line-height: 40px;
              color: #1989fa;
            "
          >
            UP
          </div>
        </el-backtop>

    </el-menu>
  </template>
  
  <script lang="ts" setup>
  import { ref } from 'vue'
  
  const activeIndex = ref('1')
  const handleSelect = (key: string, keyPath: string[]) => {
    console.log(key, keyPath)
  }
  </script>
  
  <style>
  .flex-grow {
    flex-grow: 1;
  }

  /* 去掉边框白线 */
  .el-menu {
      border-right: 0;
    }

  </style>