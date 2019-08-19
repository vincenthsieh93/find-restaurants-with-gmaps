<template>
  <div class="gmaps">
    <GmapMap :center="marker" :zoom="17" style="width: 100%; height: 100%">
      <GmapMarker :position="marker"></GmapMarker>
    </GmapMap>
  </div>
</template>

<script>
export default {
  name: "GoogleMaps",
  data () {
    return {
      marker: {lat: 23.4699739, lng: 120.9574242}
    }
  },
  mounted() {
    this.initMap();
  },
  methods: {
    initMap: function () {
      if (navigator.geolocation) {
        navigator.geolocation.getCurrentPosition(position => {
          this.marker = {
            lat: position.coords.latitude,
            lng: position.coords.longitude
          };
        }, () => {

        });
      } else {
        
      }
    }
  }
};
</script>

<style scoped lang="scss">
.gmaps {
  flex: 1;
}
</style>
