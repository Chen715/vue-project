<script setup>

import WikiHeader from'@/views/wiki/header.vue'
import wikiaside from'@/views/wiki/wikiaside.vue'
</script>

<template>
    <div class="common-layout">
      <el-container>
        <el-header>
            <WikiHeader /> 

        </el-header>
        
        <el-container class="wiki-layout-aside" >
            <el-aside width="500px" >

                <wikiaside /> 
            </el-aside>

            <el-main style="font-size: 30px" >
                Main
                <br>Main<br>Main
                <br>Main
                <br>Main
                <br>Main
                <br>Main
                <br><br>Main
                <br>Main
                <br>Main
                <br>Main
                <br>Main
                <br><br>Main
                <br>Main
                <br>Main
                <br>Main
                <br>Main
                <br><br>Main
                <br>Main
                <br>Main
                <br>Main
                <br>Main
                <br>
                <br>Main
                <br>Main
                <br>Main
                <br>Main
                <br>

            </el-main>
            
        </el-container>
      </el-container>
    </div>
  </template>

<style>

</style>
