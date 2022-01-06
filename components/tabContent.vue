<template>
<div class="custom">
<div class="p-5">
  <img class="image-wrapping px-5 " :src="data.images[0]" />
  <div class="flex pt-20 mt-0">
    <p class="number ml-0">1.
    </p>
  <p class="text mb-6 mx-5">{{data.labels[0]}}</p>
  </div>
</div>
<div class="p-5 bg-2">
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320" class="-m-5 custom-layer">
    <path fill="#fff" fill-opacity="1"  d="M0,64L60,80C120,96,240,128,360,160C480,192,600,224,720,218.7C840,213,960,171,1080,144C1200,117,1320,107,1380,101.3L1440,96L1440,0L1380,0C1320,0,1200,0,1080,0C960,0,840,0,720,0C600,0,480,0,360,0C240,0,120,0,60,0L0,0Z"></path>

</svg>
  <div class="flex pt-3 mt-0">
    <p class="number number2 ml-8">2.
    </p>
  <p class="text text2 mb-6 ml-5">{{data.labels[1]}}</p>
  </div>
  <img class="-mb-10 " :src="data.images[1]" :class="data.images[1].includes('3.2') ? 'pl-20 pr-5':(data.images[1].includes('2.2')? 'pl-10 img2 pr-10 pb-10':'pl-24 pr-11')" />
  <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320" class="-m-5 mt-5 custom-layer">
    <path fill="#fff" fill-opacity="1" class="custom-layer" d="M0,64L60,80C120,96,240,128,360,160C480,192,600,224,720,218.7C840,213,960,171,1080,144C1200,117,1320,107,1380,101.3L1440,96L1440,320L1380,320C1320,320,1200,320,1080,320C960,320,840,320,720,320C600,320,480,320,360,320C240,320,120,320,60,320L0,320Z"></path>

</svg>

</div>
<div class="rounded-full circle"></div>
<div class="p-3 pt-0 bg-3 div4">

  <div class="flex pt-0 mt-0 div3 -mt-72">
    <p class="number pl-11 ml-14">3.
    </p>
  <p class="text text3 mx-5" :class="data.images[2].includes('1.3') ? 'mb-14 ':'mb-6'">{{data.labels[2]}}</p>
  </div>
  <img class="img-3" :class="data.images[2].includes('1.3') ? '-mt-10 pl-14 img-3 ':'px-10'" :src="data.images[2]"/>
</div>
</div>
</template>

<script>
export default {
  props : {
    data: {
      type: Object,
      required: true
    }
  },

}
</script>

<style scoped>

.custom{
  /* position: relative; */
  width: 100%;
  height: 100%;
  overflow: hidden;
}
.img2{
  float: right;
  margin-top: -50px;
}
.image-wrapping
{
  float: right;
  width: auto;
  padding-left: 95px;
}
.number{
font: normal normal normal 130px Lato;
letter-spacing: 0px;
color: #718096;
margin-left: -10px;
}
.number2{
  margin-left: 15px;
}

.text{
text-align: left;
font: normal normal normal 16px/19px Lato;
letter-spacing: 0.47px;
color: #718096;
width: auto;
align-self: flex-end;
min-width: 200px;
overflow: hidden;
}
.text2{
  min-width: 182px;
}
.text3{
  min-width: 182px;
  justify-self: center;
}
.bg-2{
  background: transparent linear-gradient(134deg, #E6FFFA 0%, #EBF4FF 100%) 0% 0% no-repeat padding-box;

}
.img-3{
  shape-outside: margin-box;
}
 .div3{
  shape-outside: margin-box;
}

.custom-layer{
  z-index:10;
  position: relative;
}
.circle{
  border-radius: 50%;
  width: 350px;
  height: 303px;
  background-color: #F7FAFC;
  display: inline-block;
  margin-left: -101px;
  margin-top: -70px;
  position: relative;
  z-index: 30;
}

.div4{
  z-index: 33;
  position: relative;
}
</style>
