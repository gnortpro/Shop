<template>
  <div>
    <!-- <div class="container" id="app">
      <div class="form-group">
        <label>
          <button class="btn btn-primary btn-sm" @click.prevent="playSound(s)">
            <span class="fa fa-play-circle-o"></span>
          </button>
          Play Air Plane Ding
        </label>
      </div>
    </div>-->
    <audio controls preload="metadata">
      <source
        src="https://download1349.mediafire.com/7vknsbevs6hg/p26v2oamjq0vmiy/Dua-Nhau-Di-Tron-Chill-Version-Den-Linh-Cao.mp3"
        type="audio/mpeg"
      />
    </audio>
  </div>
</template>

<script>
export default {
  data() {
    return {
      s:
        'https://download1349.mediafire.com/7vknsbevs6hg/p26v2oamjq0vmiy/Dua-Nhau-Di-Tron-Chill-Version-Den-Linh-Cao.mp3'
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
