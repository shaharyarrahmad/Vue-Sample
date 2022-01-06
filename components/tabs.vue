<template>
  <div class="pos">
    <ul class="flex m-5 py-3">
    <li class="rounded-l-xl border px-10 py-3"  :class="curr == 1 ? 'active' : ''">
        <a  aria-current="page" @click="selected(1)">Arbeitnehmer</a>
    </li>
    <li class="border px-10 py-3" :class="curr == 2 ? 'active' : ''">
        <a class="" @click="selected(2)" >Arbeitgeber</a>
    </li>
    <li class="border px-10 rounded-r-xl py-3" :class="curr == 3 ? 'active' : ''">
        <a class="" @click="selected(3)">Temporärbüro</a>
    </li>
</ul>
  </div>
</template>

<script>

export default {
props: {
  // function as a prop
  curr: {
    type: Number,
    required: true
  },
  selected: {
    type: Function,
    required: true
  }
},
}
</script>

<style scoped>
a{
  font: normal normal 600 14px/17px Lato;
  letter-spacing: 0.84px;
  color: #319795;
}
.active{
  background-color: #2C7A7B;
  color: #fff;
}
.active a{
  color: #fff;
}
a:hover{
  /* mouse  */
  cursor: pointer;
}

.pos{
  overflow: auto;
}

::-webkit-scrollbar {
    width: 0;  /* Remove scrollbar space */
    background: transparent;  /* Optional: just make scrollbar invisible */
}
/* Optional: show position indicator in red */

</style>
