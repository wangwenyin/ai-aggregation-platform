<script setup>
const handleClick = () => {
  alert('功能开发中...')
}
</script>

<template>
  <div class="side-inner">
    <div class="btn-box">
      <div class="new-btn" @click="handleClick">新建对话</div>
      <div class="search-btn"></div>
    </div>
    <div class="current-box">
      <h5>当天</h5>
      <div class="session-list">
        <div>2024年铁路暑期结束，跨2024年铁路暑期结束，跨</div>
      </div>
    </div>
    <div class="week-box">
      <h5>最近7天</h5>
      <div class="session-list">
        <div>您擅长文章润色，文本美化。</div>
      </div>
    </div>
    <div class="manage">
      管理对话记录
    </div>
  </div>
</template>

<style scoped lang="less">
.side-inner {
  position: relative;
  padding: 32px 24px;
  font-family: AlibabaPuHuiTi_3_65_Medium;
  font-size: 14px;
  .btn-box {
    display: flex;
    margin-bottom: 25px;
    .new-btn {
      flex: 1;
      height: 36px;
      line-height: 36px;
      padding-left: 50px;
      color: #fff;
      border-radius: 18px;
      background: #5E57E6 url('@/assets/plus.png') 25% center/12px no-repeat;
      cursor: pointer;
    }
    .search-btn {
      width: 36px;
      height: 36px;
      margin-left: 5px;
      background: #FFFFFF;
      border-radius: 18px;
      border: 1px solid #E8EAF2;
      background: url('@/assets/search.png') center no-repeat;
      cursor: pointer;
    }
  }
  .current-box {
    margin-bottom: 12px;
    .session-list {
      margin-top: 12px;
      div {
        width: 100%;
        height: 36px;
        padding: 0 12px;
        line-height: 36px;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;
        background: #F3F2FF;
        border-radius: 12px;
        color: #564DD7;
        cursor: pointer;
      }
    }
  }
  .week-box {
    margin-bottom: 12px;
    .session-list {
      margin-top: 12px;
      div {
        width: 100%;
        height: 36px;
        padding: 0 12px;
        line-height: 36px;
        white-space: nowrap;
        overflow: hidden;
        text-overflow: ellipsis;
        color: #26244C;
        cursor: pointer;
        &:hover {
          color: #564DD7;
        }
      }
    }
  }
  h5 {
    font-size: 12px;
    color: #878AAB;
  }
  .manage {
    position: absolute;
    left: 0;
    bottom: 0;
    width: 100%;
    height: 56px;
    line-height: 56px;
    padding-left: 45px;
    border-top: 1px solid #E8EAF2;
    background: url('@/assets/manage.png') 10% center no-repeat;
    cursor: pointer;
  }
}
</style>
