<template>
<div class="w-100 header">
<div class="w-100 bg-black height"></div>
<div class="w-100 bg-black login-height flex flex-row-reverse">
  <t-button class="login-button m-5" variant="link">
    Login
  </t-button>
</div>
</div>
</template>

<script>
import TButton from 'vue-tailwind/dist/t-button'
export default {
  components: {
    TButton
  }
}
</script>

<style scoped>
.height {
height:  5px;
background: transparent linear-gradient(91deg, #319795 0%, #3182CE 100%) 0% 0% no-repeat padding-box;
}
.login-height {
height:  62px;
background: #FFFFFF 0% 0% no-repeat padding-box;
box-shadow: 0px 3px 6px #00000029;
border-radius: 0px 0px 12px 12px;

}
.login-button {
text-align: left;
font: normal normal 600 14px/17px Lato;
letter-spacing: 0.84px;
color: #319795;
}
.header {
   position: sticky;
   top: 0;
   z-index: 100;
}

</style>
