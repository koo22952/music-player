<template>
  <div class="music-top__left" :style="songImg">
    <div class="mask"></div>
    <div class="personal_info">
      <div class="info">
        <p class="info_Career">ARTIST</p>
        <p class="info_name">ED SHEERAN</p>
      </div>
      <div class="flowersMeg">
        <div class="followers">
          <span>4,242,424</span>
          <span>Followers</span>
        </div>
        <div class="btngroup">
          <button class="btn followBtn">FOLLOWING</button>
          <button class="btn playBtn">PLAY</button>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    data() {
      return {
        Imgdata: `url(${require('@/assets/img/astist_photo.png')})`
      }
    },
    computed: {
      songImg() {
        return { backgroundImage: this.Imgdata }
      }
    },
  }
</script>

<style lang="scss" scoped>
  .music-top__left {
    width: 39%;
    // flex: 1;
    background-size: cover;
    background-position: center center;
    background-repeat: no-repeat;
    overflow: hidden;
    display: flex;
    align-items: flex-end;
    position: relative;
    text-transform: uppercase;
    .mask {
      position: absolute;
      width: 100%;
      height: 263px;
      background: linear-gradient(rgba(0, 0, 0, 0), black);
      z-index: 1;
    }
    .personal_info {
      padding: 31px;
      padding-left: 62px;
      width: 100%;
      z-index: 2;
      .info {
        margin-bottom: 21px;
        &_Career {
          color: #e5b4b7;
          font-size: 14px;
          margin: 0;
        }
        &_name {
          font-size: 24px;
          color: white;
          font-weight: bold;
          margin: 0;
          margin-top: 5px;
        }
      }
      .flowersMeg {
        display: flex;
        justify-content: space-between;
        align-items: flex-end;
        .followers {
          display: flex;
          flex-direction: column;
          font-size: 11px;
          color: #ffffff;
          text-transform: capitalize;
          span {
            line-height: 16px;
          }
        }
        .btngroup {
          .btn {
            width: 128px;
            height: 30px;
            border-radius: 17px;
            font-size: 14px;
            border: none;
            font-weight: bold;
          }
          .followBtn {
            margin-right: 17px;
            background-color: transparent;
            border: 1px solid #ffff;
            color: #964a4d;
          }
          .playBtn {
            background-color: #964a4d;
            color: #ffffff;
            border: 1px solid #964a4d;
          }
        }
      }
    }
  }
</style>
