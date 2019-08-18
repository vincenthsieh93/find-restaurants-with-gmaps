<template>
  <div class="gmaps">
    <GmapMap :center="{lat: 22.891308, lng: 120.242871}" :zoom="17" style="width: 100%; height: 100%"></GmapMap>
  </div>
</template>

<script>
export default {
  name: "GoogleMaps"
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.gmaps {
  flex: 1;
}
</style>
