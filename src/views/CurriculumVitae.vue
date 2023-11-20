<script setup lang="ts">
import ContentHead from '../components/ContentHead.vue'
import selfPic from '@/assets/images/self-pic.png'
</script>

<template>
  <div class="outer-wrap">
    <div class="header-area">实事求是，敢为人先</div>
    <div class="content-warp">
      <ContentHead headTitle="个人信息"></ContentHead>
      <div class="basic-wrap">
        <div class="basic-content-left">
          <div class="item-wrap">
            <div class="item-title"><span>姓名</span>：</div>
            <div class="item-content isBold">李显</div>
          </div>
          <div class="item-wrap">
            <div class="item-title"><span>身高</span>：</div>
            <div class="item-content">180cm</div>
          </div>
          <div class="item-wrap">
            <div class="item-title"><span>联系电话</span>：</div>
            <div class="item-content">135200382238</div>
          </div>
          <div class="item-wrap">
            <div class="item-title"><span>职位</span>：</div>
            <div class="item-content isBold">前端开发</div>
          </div>
        </div>
        <div class="basic-content-right">
          <div class="item-wrap">
            <div class="item-title"><span>出生年月</span>：</div>
            <div class="item-content">1990.9</div>
          </div>
          <div class="item-wrap">
            <div class="item-title"><span>现居地</span>：</div>
            <div class="item-content">北京</div>
          </div>
          <div class="item-wrap">
            <div class="item-title"><span>电子邮件</span>：</div>
            <div class="item-content">wangyi_lixian@163.com</div>
          </div>
        </div>
        <div class="basic-img-wrap">
          <img :src="selfPic" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.outer-wrap {
  border: 1px solid #ccc;
  width: 210mm;
  height: 100vh;
  color: #333;
  overflow-y: auto;
  padding: 0 20mm;
}
.outer-wrap .header-area {
  color: #333;
  font-size: 24px;
  padding: 6mm 0;
  text-align: center;
  font-family: 'Microsoft YaHei UI';
  position: relative;
}
.outer-wrap .header-area::before {
  position: absolute;
  content: '';
  width: 30px;
  height: 30px;
  border-width: 0 1px 1px 0;
  border-style: solid;
  border-color: #ccc;
  left: -16mm;
  bottom: 0;
}
.outer-wrap .header-area::after {
  position: absolute;
  content: '';
  width: 30px;
  height: 30px;
  border-width: 0 0 1px 1px;
  border-style: solid;
  border-color: #ccc;
  right: -16mm;
  bottom: 0;
}
.outer-wrap .content-warp {
  height: 297mm;
}
.outer-wrap .content-warp .basic-wrap {
  padding: 16px 48px 16px 0;
  display: flex;
  position: relative;
}
.outer-wrap .content-warp .basic-wrap .basic-content-left {
  margin-right: 72px;
}
.basic-content-right {
  /*border: 1px solid blue;*/
}
.outer-wrap .content-warp .basic-wrap .item-wrap {
  display: flex;
}
.outer-wrap .content-warp .basic-wrap .item-wrap .item-title > span {
  display: inline-block;
  width: 64px;
  text-align: justify;
  text-align-last: justify;
}
.outer-wrap .content-warp .basic-wrap .item-wrap .item-content.isBold {
  font-size: 16px;
  font-weight: 600;
}
.outer-wrap .content-warp .basic-wrap .basic-img-wrap {
  width: 90px;
  height: 120px;
  position: absolute;
  top: 4px;
  right: 16px;
}
.outer-wrap .content-warp .basic-wrap .basic-img-wrap img {
  width: 100%;
  height: 100%;
}
</style>
