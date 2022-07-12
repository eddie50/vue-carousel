<template>
  <div class="carousel-indicators">
    <button class="carousel-indicator-item"
    v-for="(item,i) in count"
    :key="i"
    :class="{active: active === i}"
    @click="$emit('switch',i)"
    ></button>
  </div>
</template>

<script>
export default {
    emits:['switch'],
    props:['count','active']
}
</script>

<style scoped>

.carousel-indicators{
    position: absolute;
    bottom: 1.5em;
    z-index: 2;
    transform: translateX(-50%);
    left: 50%;
}
.carousel-indicator-item{
    border: none;
    padding: 0;
    width: 15px;
    height: 15px;
    background: #fff;
    border-radius: 50%;
    opacity: 0.5;
    margin: 0.2em;
    cursor: pointer;
}
.active{
    opacity: 1;
}
</style>