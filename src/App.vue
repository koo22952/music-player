<template>
  <div id="app">
    <div class="music">
      <div class="music-top">
        <coverPicture></coverPicture>
        <list></list>
      </div>
      <div class="music-down">
        <playBar />
      </div>
    </div>
    <aaaaa></aaaaa>
  </div>
</template>

<script>
  import coverPicture from './components/coverPicture'
  import list from './components/list'
  import playBar from './components/playBar'
  import aaaaa from './components/navbar'

  export default {
    name: 'app',
    components: {
      coverPicture,
      list,
      playBar,
      aaaaa,
    },
  }
</script>

<style lang="scss">
  @import "./assets/all.scss";

  #app {
    width: 100%;
    display: flex;
    .music {
      width: calc(100% - 80px);
      .music-top {
        height: calc(100vh - 100px);
        display: flex;
      }
      .music-down {
        min-height: 100px;
      }
    }
  }
</style>
