<script lang="ts" setup>
import { defineProps } from "vue"
import {Articles} from "@/types/articles";

interface Props {
  articleData: Array<Articles>
}
const props = withDefaults(defineProps<Props>(), {
  articleData: () => []
})
console.log(props);
</script>
<template>
  <article class="w-full h-full">
    <section class="meta-wrapper flex items-center flex-col">
      <div class="item-wrapper">
        <div class="title text-center">
          <p class="font-black text-xl">测试标题</p>
        </div>
        <div class="meta">
        </div>
        <div class="date">
          <p class="text-center">5月</p>
          <p class="text-center">29</p>
        </div>

      </div>
    </section>
    <section class="meta-wrapper flex items-center flex-col">
      <div class="item-wrapper">
        <div class="title text-center">
          <p class="font-black text-xl">测试标题</p>
        </div>
        <div class="meta">

        </div>
        <div class="date">
          <p class="text-center">5月</p>
          <p class="text-center">29</p>
        </div>
      </div>
    </section>
    <section class="meta-wrapper flex items-center flex-col">
      <div class="item-wrapper">
        <div class="title text-center">
          <p class="font-black text-xl">测试标题</p>
        </div>
        <div class="meta">

        </div>
        <div class="date">
          <p class="text-center">5月</p>
          <p class="text-center">29</p>
        </div>
      </div>
    </section>
  </article>
</template>

<style scoped lang="scss">

    .meta-wrapper{
      width: 100%;


      .item-wrapper {
        background: #FFFFFF;
        margin: 20px;
        padding: 10px;
        border-radius: 3px;
        width: 60%;
        position: relative;

        &:first-child {
          margin-top: 60px;
        }


        .date {
          background: #07c160;
          position: absolute;
          top: -20px;
          left: -20px;
          width: 50px;
          height: 50px;
          border-radius: 50%;
        }

        .title {

        }

        .meta {

          height: 300px;
        }
      }

    }
</style>