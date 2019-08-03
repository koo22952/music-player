<template>
  <div class="musicNavbar">
    <div class="avatar"></div>
    <div class="menuIcon">
      <img src="../assets/svg/home-52.svg" />
      <img src="../assets/svg/archive-2.svg" />
      <img src="../assets/svg/ic_library_music_48px.svg" />
    </div>
    <div class="menuSearch">
      <img src="../assets/svg/zoom-2.svg" />
      <img src="../assets/svg/settings-gear-63.svg" />
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .musicNavbar {
    min-width: 80px;
    background: #4b3434;
    text-align: center;
    padding: 50px 0 43px 0;
    position: relative;
    .avatar {
      width: 56px;
      height: 56px;
      background-color: #707070;
      border-radius: 50%;
      margin: 0 auto;
      margin-bottom: 57px;
    }
    .menuIcon {
      display: flex;
      flex-direction: column;
      img {
        &:nth-child(2) {
          margin: 64px 0;
        }
      }
    }
    .menuSearch {
      position: absolute;
      bottom: 43px;
      left: 50%;
      transform: translate(-50%, 0);
      display: flex;
      flex-direction: column;
      img {
        &:nth-child(2) {
          margin-top: 28px;
        }
      }
    }
  }
</style>
