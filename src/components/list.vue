<template>
  <div class="music-top__right">
    <div class="musicinfo">
      <img src="../assets/img/Ed_Sheeran_-_No._6_Collaborations_Project@2x.png" alt />
      <div class="musicinfo-title">
        <div>
          <span>2019</span>
          <h2>No.6 Collaborations Project</h2>
        </div>
        <button>PLAY</button>
      </div>
      <div class="musicinfo-heart">
        <img src="../assets/svg/heart-2.svg" alt />
      </div>
    </div>
    <div class="musicList">
      <table>
        <tr>
          <th width="50px"></th>
          <th width="60px"></th>
          <th style="text-align:left">title</th>
          <th width="60px">length</th>
          <th width="200px">
            <img src="../assets/svg/heart-2-2.svg" alt />
          </th>
        </tr>
        <tr>
          <td>
            <img src="../assets/svg/ic_music_note_24px.svg" alt />
          </td>
          <td>
            <span>1</span>
          </td>
          <td>Beautiful People</td>
          <td>3:17</td>
          <td>
            <span>12,523</span>
            <img src="../assets/svg/heart-2-1.svg" alt />
          </td>
        </tr>
        <tr>
          <td></td>
          <td>
            <span>2</span>
          </td>
          <td>South of the Border</td>
          <td>3:24</td>
          <td>
            <span>33,213</span>
            <img src="../assets/svg/heart-2.svg" alt />
          </td>
        </tr>
      </table>
    </div>
  </div>
</template>
<script>

  export default {
    components: {
    }
  }
</script>

<style lang="scss" scoped>
  .music-top__right {
    flex: 1;
    background-color: #1a1a1a;
    text-transform: capitalize;
    display: flex;
    flex-direction: column;
    overflow: hidden;
    .musicinfo {
      display: flex;
      padding: 0px 64px 42px 42px;
      > img {
        width: 90px;
        height: 90px;
        margin-right: 53px;
        padding-top: 89px;
      }
      &-title {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        padding-top: 75px;
        span {
          font-size: 14px;
          color: #707070;
        }
        h2 {
          margin: 0;
          font-size: 32px;
          color: #ffffff;
        }
        > button {
          width: 128px;
          color: #ffffff;
          font-weight: bold;
          background-color: #964a4d;
          border: 1px solid #964a4d;
          border-radius: 17px;
          padding: 6px 20px;
        }
      }
      &-heart {
        display: flex;
        align-items: flex-end;
        margin-bottom: 10px;
        margin-left: auto;
        margin-right: 17px;
        img {
          width: 24px;
          height: 22px;
        }
      }
    }
    .musicList {
      overflow-y: scroll;
      table {
        color: #ffffff;
        text-align: center;
        border-spacing: 0;
        width: 100%;
        th,
        td {
          padding-bottom: 9px;
          border-bottom: 0.2px solid #707070;
        }
        th {
          font-size: 14px;
          color: #964a4d;
          font-weight: 400;
          text-transform: uppercase;
        }
        td {
          padding: 17px 0 14px 0;
          font-size: 14px;
          &:nth-child(2),
          &:nth-child(3) {
            text-align: left;
            font-size: 18px;
          }
          &:last-child {
            span {
              margin-right: 14px;
            }
            img {
              vertical-align: text-top;
            }
          }
        }
      }
    }
  }

  /* 设置滚动条的样式 */
  ::-webkit-scrollbar {
    width: 5px;
  }

  /* 滚动条滑块 */
  ::-webkit-scrollbar-thumb {
    border-radius: 10px;
    background: rgba(150, 74, 77, 0.8);
  }
</style>
