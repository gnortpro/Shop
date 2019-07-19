<template>
  <div>
    <div class="container" id="app">
      <div class="form-group">
        <label>
          <button class="btn btn-primary btn-sm" @click.prevent="playSound(s)">
            <span class="fa fa-play-circle-o"></span>
          </button>
          Play Air Plane Ding
        </label>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      s:
        'https://vnno-vn-6-tf-mp3-s1-zmp3.zadn.vn/8fd0d56eae2a47741e3b/5253865936530607617?authen=exp=1563605386~acl=/8fd0d56eae2a47741e3b/*~hmac=d4d2d44e02dba8edbcd25c5c664b7f43&filename=Dua-Nhau-Di-Tron-Chill-Version-Den-Linh-Cao.mp3'
    }
  },
  methods: {
    playSound(sound) {
      if (sound) {
        var audio = new Audio(sound)
        audio.play()
      }
    }
  }
}
</script>

<style>
</style>
