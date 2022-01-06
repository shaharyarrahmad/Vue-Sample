<template>
<div>
    <div>
  <p class="header">{{tabInfo.header}}</p>
  <h1 class="header px-11">{{tabInfo.h2}}</h1>
  <tabContent :data="tabInfo"></tabContent>
</div>
<!-- <div class="div2 number">.</div> -->


</div>
</template>

<script>
import tabContent from '../components/tabContent.vue'
export default {
  props: {
    // function as a prop
    tabInfo: {
      type: Object,
      required: true
    }
  },
}
</script>
<style scoped>
.header{
text-align: center;
font: normal normal 300 21px/25px Lato;
letter-spacing: 0px;
color: #4A5568;
align-self: flex-end;
min-width: max-content;
}
/* display text and image in line */


</style>
