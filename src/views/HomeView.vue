<script setup>
import TheWelcome from '../components/TheWelcome.vue'
</script>

<template>
  <div class="main">
    <div class="content">
      <div class="top">
        <h2>你好，我是AI聚合<br>让我们一起度过美好的一天</h2>
        <div class="recomend">
          <div class="please">
            <span>你可以尝试下面的示例…</span>
            <div class="refresh">换一换</div>
          </div>
          <div class="card-box">
            <img src="" alt="">
            <img src="" alt="">
            <img src="" alt="">
          </div>
        </div>
      </div>
      <div class="footer">
        <div class="send-message-box">
          <div class="tags">
            <div>帮我写作</div>
            <div>图片生成</div>
            <div>阅读总结</div>
            <div>解题答疑</div>
            <div>翻译</div>
            <div>网页摘要</div>
          </div>
          <div class="input-box">
            <input type="text" placeholder="发消息、输入@或/选择技能">
          </div>
        </div>
        <div class="copy-right">服务生成的所有内容均由人工智能模型生成，其生成的内容的准确性和完整性无法保证，不代表我们的态度或观点</div>
      </div>
    </div>
  </div>
</template>

<style scoped lang="less">
.main {
  flex: 1;
  background: linear-gradient( 180deg, #EFEEFD 0%, #FFFFFF 100%);
  border-radius: 0px 10px 10px 0px;
  .content {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    width: 60%;
    height: calc(90vh - 90px);;
    margin: 10vh auto 0;
    .top {
      padding: 0 60px;
      h2 {
        font-family: AlibabaPuHuiTi_3_85_Bold;
        font-size: 27px;
        color: #2C2C36;
        line-height: 38px;
        text-align: left;
        font-style: normal;
      }
      .recomend {
        margin-top: 30px;
        .please {
          display: flex;
          justify-content: space-between;
          margin-bottom: 10px;
          font-size: 14px;
          color: #8F91A8;
          .refresh {
            padding-left: 18px;
            background: url('@/assets/refresh.png') left center/13px no-repeat;
            color: #564DD7;
            cursor: pointer;
          }
        }
        .card-box {
          display: flex;
          img {
            flex: 1;
            height: 30vh;
            margin-right: 15px;
            background: linear-gradient( 180deg, #5B56F6 0%, #908DFF 34%, #CCCAFB 69%, #F6F6FF 100%);
            border-radius: 16px;
            &:last-child {
              margin-right: 0;
            }
          }
        }
      }
    }
    .footer {
      .send-message-box {
        .tags {
          display: flex;
          div {
            width: 100px;
            height: 30px;
            line-height: 30px;
            padding-left: 30px;
            margin-left: 8px;
            background: #FFFFFF;
            border-radius: 8px;
            border: 1px solid #E8EAF2;
            cursor: pointer;
          }
        }
        .input-box {
          margin-top: 8px;
          input {
            width: 100%;
            height: 40px;
            padding: 0 50px;
            border-radius: 16px;
            border: 1px solid #E8EAF2;
            background: url('@/assets/link.png') 2% center no-repeat,
                        url('@/assets/jd.png') 94% center no-repeat,
                        url('@/assets/ht.png') 98% center no-repeat;
            &:focus {
              outline: #5B56F6;
            }
          }
        }
      }
      .copy-right {
        width: 100%;
        height: 35px;
        line-height: 35px;
        text-align: center;
        font-size: 10px;
        color: #8F91A8;
      }
    }
  }
}
</style>
