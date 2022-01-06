<template>
<div class="block px-5 podbar">
  <t-button class="gradiant my-5">
   <p class="m-1">
         Kostenlos Registrieren
    </p>
  </t-button>
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
.block {
  display: block;
  background-color: #FFFFFF;
  box-shadow: 3px 0px 6px #00000029;
  border-radius: 12px 12px 0px 0px;
  padding: 10px;
  font: normal normal 600 14px/17px Lato;
  letter-spacing: 0.84px;
}
.gradiant {
  background: transparent linear-gradient(95deg, #319795 0%, #3182CE 100%) 0% 0% no-repeat padding-box;
border-radius: 12px;
width: 100%;
}
.gradiant:hover{
  background: transparent linear-gradient(95deg, #2C7A7B 0%, #2B6CB0 100%) 0% 0% no-repeat padding-box;
}
.podbar {
    bottom:0;
    position:sticky;
    z-index:150;
    width:100%;
}
</style>
