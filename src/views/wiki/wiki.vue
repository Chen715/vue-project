<script setup>

import WikiHeader from'@/views/wiki/header.vue'
import wikiaside from'@/views/wiki/wikiaside.vue'
import wikiheader2 from'@/views/wiki/wiki_header2.vue'

import wikimain from'@/views/wiki/wikimain.vue'
import cebianlan from'@/views/wiki/cebianlan.vue'

import { reactive, watch } from 'vue'
  
  const font = reactive({
    color: 'rgba(0, 0, 255, .15)',
  })
</script>

<template>
    <div class="common-layout">
      <el-container>
        <el-header>
            <WikiHeader /> 

        </el-header>
        <el-header>
          <el-affix>
            <!-- 固钉 固定顶部的位置 -->
            <wikiheader2 /> 
          </el-affix>
        </el-header>
        
        <el-container class="wiki-layout-aside" >
          
          <el-affix :offset="60">
            <el-aside width="250px">
                <wikiaside /> 
            </el-aside>

          </el-affix>


            <el-main >
              <el-watermark :font="font" :content="['Element+', 'Element Plus']">
                <wikimain /> 
              </el-watermark>
              
            </el-main>

            
        </el-container>

        
            
      <el-footer>Footer</el-footer>
      </el-container>
    </div>
  </template>

<style>
  body{
    margin: 0px;
  }

  .el-header {
        position: relative;
        width: 100%;
        height: 60px;      
    }

  .el-aside {
  display: block;
  position: absolute;
  left: 0;
  top: 60px;
  bottom: 0;
  }

  .el-main {
  position: absolute;
  left: 200px;
  right: 0;
  top: 60px;
  bottom: 0;
  overflow-y: scroll;
  }


</style>
