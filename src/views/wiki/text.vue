<template>
  <div>
    <el-row>
      <el-col :span="18">
        <div
          style="
            height: 30px;
            width: 70%;
            background: #000;
            position: absolute;
            top: 0;
            left: 0;
            color: #fff;
          "
        >
          Fixed Top Block
        </div>
        <div ref="containerRef" style="height: 300px; overflow-y: auto">
          <div
            id="part1"
            style="
              height: 300px;
              background: rgba(255, 0, 0, 0.02);
              margin-top: 30px;
            "
          >
            part1
          </div>
          <div
            id="part2"
            style="
              height: 300px;
              background: rgba(0, 255, 0, 0.02);
              margin-top: 30px;
            "
          >
            part2
          </div>
          <div
            id="part3"
            style="
              height: 300px;
              background: rgba(0, 0, 255, 0.02);
              margin-top: 30px;
            "
          >
            part3
          </div>
        </div>
      </el-col>
      <el-col :span="6">
        <el-anchor
          :container="containerRef"
          direction="vertical"
          type="defalut"
          :offset="30"
          @click="handleClick"
        >
          <el-anchor-link href="#part1" title="part1" />
          <el-anchor-link href="#part2" title="part2" />
          <el-anchor-link href="#part3" title="part3" />
        </el-anchor>
      </el-col>
    </el-row>
  </div>

  字数的多少，是区别长篇、中篇、短篇小说的一个因素。但不是惟一的因素。人们通常把五千到一万五千字的小说称为短篇小说，三万字到十万字的小说称为中篇小说，十万字以上的称为长篇小说。这只是就字数而言的，其实，长、中、短篇小说的区别，主要是由作品反映生活的范围、作品的容量来决定的。长篇小说容量最大，最广阔，篇幅也比较长，具有比较复杂的结构，它一般是通过比较多的人物和纷繁的事件来表现社会生活的，如《红楼梦》。中篇小说反映生活的范围虽不像长篇那样广阔，但也能反映出一定广度的生活面，它的人物的多寡、情节的繁简介于长篇与短篇之间，如《人到中年》。短篇小说的特点是紧凑、短小精悍，它往往只写了一个或很少几个人物，描写了生活的一个片断或插曲。短篇小说所反映的生活虽不及长篇、中篇广阔，但也同样是完整的，有些还具有深刻、丰富的社会意义。
              字数的多少，是区别长篇、中篇、短篇小说的一个因素。但不是惟一的因素。人们通常把五千到一万五千字的小说称为短篇小说，三万字到十万字的小说称为中篇小说，十万字以上的称为长篇小说。这只是就字数而言的，其实，长、中、短篇小说的区别，主要是由作品反映生活的范围、作品的容量来决定的。长篇小说容量最大，最广阔，篇幅也比较长，具有比较复杂的结构，它一般是通过比较多的人物和纷繁的事件来表现社会生活的，如《红楼梦》。中篇小说反映生活的范围虽不像长篇那样广阔，但也能反映出一定广度的生活面，它的人物的多寡、情节的繁简介于长篇与短篇之间，如《人到中年》。短篇小说的特点是紧凑、短小精悍，它往往只写了一个或很少几个人物，描写了生活的一个片断或插曲。短篇小说所反映的生活虽不及长篇、中篇广阔，但也同样是完整的，有些还具有深刻、丰富的社会意义。
              字数的多少，是区别长篇、中篇、短篇小说的一个因素。但不是惟一的因素。人们通常把五千到一万五千字的小说称为短篇小说，三万字到十万字的小说称为中篇小说，十万字以上的称为长篇小说。这只是就字数而言的，其实，长、中、短篇小说的区别，主要是由作品反映生活的范围、作品的容量来决定的。长篇小说容量最大，最广阔，篇幅也比较长，具有比较复杂的结构，它一般是通过比较多的人物和纷繁的事件来表现社会生活的，如《红楼梦》。中篇小说反映生活的范围虽不像长篇那样广阔，但也能反映出一定广度的生活面，它的人物的多寡、情节的繁简介于长篇与短篇之间，如《人到中年》。短篇小说的特点是紧凑、短小精悍，它往往只写了一个或很少几个人物，描写了生活的一个片断或插曲。短篇小说所反映的生活虽不及长篇、中篇广阔，但也同样是完整的，有些还具有深刻、丰富的社会意义。

</template>

<script setup lang="ts">
import { ref } from 'vue'

const containerRef = ref<HTMLElement | null>(null)

const handleClick = (e: MouseEvent) => {
  e.preventDefault()
}
</script>
