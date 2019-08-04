<template>
  <div class="music-down">
    <div class="playBar">
      <div style="width: 30%"></div>
    </div>
    <div class="controlPanel">
      <div class="music-time">
        <span>1:38</span>
        <span>3:39</span>
      </div>
      <div class="music-doing">
        <div class="info">
          <img src="../assets/img/Ed_Sheeran_-_No._6_Collaborations_Project@2x.png" alt />
          <div class="info-detail">
            <span class="song">I Don’t Care</span>
            <span class="singer">Ed Sheehan (with Justin Bieber)</span>
          </div>
        </div>
        <div class="controlStrip">
          <img src="../assets/svg/btn_shuffle.svg" />
          <img src="../assets/svg/btn_play_Left.svg" />
          <img src="../assets/svg/btn_start.svg" />
          <img src="../assets/svg/btn_play_Right.svg" />
          <img src="../assets/svg/btn_repeat.svg" />
        </div>
        <div class="controlOther">
          <div class="controlOther-Voice">
            <img src="../assets/svg/btn_volume_up.svg" />
            <div>
              <div style="width: 54%;"></div>
            </div>
          </div>
          <div class="controlOther-heart">
            <img src="../assets/svg/heart-2.svg" alt />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {

  }
</script>

<style lang="scss" scoped>
  .music-down {
    width: 100%;
    .playBar {
      height: 12px;
      background-color: #ffffff;
      border: 1px solid #ffffff;
      box-sizing: border-box;
      > div {
        height: 10px;
        background-color: #e5b4b7;
      }
    }
    .controlPanel {
      height: 87px;
      background: linear-gradient(#772020, #361024);
      display: flex;
      flex-direction: column;
      color: #ffffff;
      & .music-time {
        font-size: 12px;
        padding: 5px 24px 3px;
        display: flex;
        justify-content: space-between;
      }
      & .music-doing {
        display: flex;
        align-items: center;
        padding: 0 74px 12px;
        .info {
          width: 25%;
          display: flex;
          img {
            width: 40px;
            height: 40px;
            margin-right: 20px;
          }
          &-detail {
            display: flex;
            flex-direction: column;
            font-size: 12px;
            justify-content: space-around;
            .song {
              font-size: 20px;
              font-weight: bold;
            }
          }
        }
        .controlStrip {
          width: 50%;
          display: flex;
          justify-content: center;
          img {
            margin: 0 10px;
            &:first-child {
              margin-right: 35px;
            }
            &:last-child {
              margin-left: 35px;
            }
          }
        }
        .controlOther {
          width: 25%;
          display: flex;
          justify-content: flex-end;
          &-Voice {
            display: flex;
            align-items: center;
            > div {
              width: 100px;
              height: 6px;
              border-radius: 3px;
              background-color: #ffffff;
              margin-left: 9px;
              border: 1px solid #ffffff;
              div {
                height: 6.5px;
                border-radius: 3px;
                background-color: #964a4d;
              }
            }
          }
          &-heart {
            margin-left: 54px;
            img {
              width: 24px;
            }
          }
        }
      }
    }
  }
</style>
