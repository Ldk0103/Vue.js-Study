<script>
export default {
  // function 생략가능 (ES6 문법)
  data : function() {
    return {
      header : '<a href="https://youtube.com" target="blank">첫 Vue.js 독학</a>',
      name : '철수',
      age : 19,
      color : 'red-color',
      class : 'blue-color',
      score : 69,
    };
  }, 
}
</script>
<template>
  <div v-html="header"></div>
  <p>내 이름은 {{ name }} 입니다.</p>
  <p>나이는 {{ age }} 살 입니다.</p>

  <!--외부 속성에 데이터 연결하는 디렉티브 v-bind -->
  <div v-bind:class="color">안녕</div>
  <!--디렉티브 v-bind 축약형/ vue3.4~ 이상이면 속성과 이름이 같으면 단축 가능 -->
  <div :class="color">안녕</div>
  <div :class>안녕</div>

  <div v-if="score === 80">시험 점수가 80점 입니다.</div>
  <div v-else-if="score === 70">시험 점수가 70점 입니다.</div>
  <div v-else="score < 70">시험 점수가 {{score}}점 입니다.</div>
</template>
<style>
.red-color {
  color:red;
}
.blue-color {
  color:blue;
}
</style>