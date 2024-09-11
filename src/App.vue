<script setup>
import { RouterLink, RouterView } from 'vue-router'
import SideBar from './components/SideBar.vue'
</script>

<template>
  <header>
    <div class="logo">
      <img src="@/assets/logo.png" alt="">
      <span class="title">AI聚合平台</span>
    </div>
    <div class="quick-start">
      <div>
        <div class="box talk current">
          <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAGKADAAQAAAABAAAAGAAAAADiNXWtAAABgklEQVRIDe2VsUoDQRCGcxIEX0GSwkKwsRDRxhSihV0EtfAV8go2wfgQeQuLIKhNsFWSSrBRsRAsrBQU7c5vjt1zb527w9zaufBnZ/6Z+Wdv9zZXq/2Pkh2IbDyO4yb2Opix3ITzB3UXURQ9pvWIt8A7CDVEq+U2GIRSdnQG0mDKdJlNu4UzEk3bIJysp1TW4Ib8I/Ds1YkrXA9ITvFg30bO3rlmWyohei5p7EMTaysxoUYSr8tPweiQKOFdJWeP2Bi+o8SylHQDoUfyBGVnkF3JBJ5tkN5oT+MMfxucery4J0DO6FycvGHPINloJanPlZcLIxdxnnnR5FzD34oNL4vcMrw+kTTOOYBL+IZelYg3iV/l1GbeorwnWEX8HoFj5iF4MM3mmDfADpg2nDrZLVKDhhSBfYOiPDVmD/lJjVYjvzXZgj/7u05fT5rYD84CCz/wFv+J3wUvHq+5Pz84bhaNloE73nA23ZxKNmJLjvor9lolQb8YwToYgjuw4sd/638Bx+BQdsMHwHEAAAAASUVORK5CYII=" class="label_2">
        </div>
        <span>对话</span>
      </div>
      <div>
        <div class="box write">
          <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAGKADAAQAAAABAAAAGAAAAADiNXWtAAABPElEQVRIDWNgGOzg////ikDcC8SJVHcr0FBpIH4LxDDQRTVLgCYKA3ESzGQkmnJLgIYpAfEjIO4C4kIgRgftZPsEaBLMcJih2Cz5C5SUJNkSLIbjsuQpUIKZJAvwGI5uCSjSDaltOMySaiBDhFaGPwcarjFqOCysYfTgCxZQ9gflUEKAaJczocW6HZC/Ak0MnfsCKODIyMh4A10CLx/oZBkg/gfEoLIFlP2xAaJdjmEZ0LQ0JBOxWUK+4SDbgIZvQLIAxES2hGzDGaGGswHpd0DMDeIjgSIgmwuI15Ic5kiGgFzviuZ6EPcaEPcBMQ+yWlLZMB9MA2oE1akPgPgeFH8C0jDwCeiDThAHaCEvkKqASeCgbwHVLwTJsUAVLAHSoAriP5QvDaRBGAZAwQcDID2aMA4O+gcOceoLAwChHcPKW0DEbAAAAABJRU5ErkJggg==" class="label_3">
        </div>
        <span>帮我写作</span>
      </div>
      <div>
        <div class="box img">
          <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAGKADAAQAAAABAAAAGAAAAADiNXWtAAABUUlEQVRIDd2VPU7DQBCFbaBMSiiouAW0SFDRcAckCq6BRB+OA4VDAQWcAhp6RBlkvrd4nImzGxNvGhjpZX52573xbqQtin9jdV1PwAzkmjgmdjClBRRnxNuWZ/qvsix3xLHliDZFLsqWyws4reKN5BSMG698kKUELmA7Bu+NVz7I/B3UjkGTi3wEPsE++AC/Nu4gcKe+4AimWyBy+UOQZ53/5iv5CRg1XvlatjTNWt3zzU+El+B5XvqJTCB1RLa+yt+zeA4OwBl4AGnrTtCT37G+Bx6bfVP8LpAPtqRkC87rs6/Ai6sp7JLbssglGkT6BCo2aqJr0DYRp8hZCtaKrBKo2Oo/15puqPtjCYyRn7A/JVDR4MmtX+RjYGdu9ZSfxgQqdsfI+44lKhIT2Bi5FGMC4fbdOIMmt/6YgH/NssgR0eO1aBTtycwmF9ci+1/OvgH3R/1NH1bRHAAAAABJRU5ErkJggg==" class="label_4">
        </div>
        <span>图片生成</span>
      </div>
      <div>
        <div class="box read">
          <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAYAAADgdz34AAAAAXNSR0IArs4c6QAAAERlWElmTU0AKgAAAAgAAYdpAAQAAAABAAAAGgAAAAAAA6ABAAMAAAABAAEAAKACAAQAAAABAAAAGKADAAQAAAABAAAAGAAAAADiNXWtAAACV0lEQVRIDdWVS0hVURSGPRAYKllBEjQL0oEQhIL0AGvSc1gEPSZhBCVKgwbSA4yiIBsKUdAoBzYJHCha0GkYNGjirKBBRSBRJCJCj+33b9c6HQ/ec8+kQT98d6299r/W3fe6z7Wh4X9XUvUDhBBa8F40/4MkSRaq9lby8QYT4Jqo1FTVxNTdNvkjUUh7qvbX9TFsOo4MoZ8opOm6jVUMDOqJ40L4TGw0lEs9VWaUehgyGUeFMOhG1oNWm1SNPIGrMA4b3aeY3SI2trHWiXbkaCffCl9gOzdniaiB6wkfoA1OwGG4ANIxeItXPSui4TT8gqL+UPgE593rUTU4Bw/B9YrkJPyEU+7ViZ6D9BqG4DjshCaZiJszsyXU9LUUh7dS81kzWQ/FAZDmYV+2QcL6jDbQmNfJNfyRiiadvBn2wg+rZX+z2Efxnm0sEA/khl2yusJZKA5PqTXBflCvdN/7V0U2bsXtEBaJh7RJ1NWctfo34pjlCilo+EFQj3R71dDiAsP1aAthiXjE3qSbvHgJUmoafhTklW4U5625xjga7SGMuIH1HaspvAS/ACNWH3VvPq7LL3J5sHw2Vxsmbwb9qg5wzxeJknu8Z6Va9sqJUjtVV5lPe/i6zJvW82b7NMzBb4hfgw3axXoKZqDbzfKAvHNeK40Y20B6Z4M7yJ+Cnuq8nrHoNM9729BPR7kw9ppZT/Vj8NvzlfwKXAZ9QkknfwJvtEC95dPZxdQZrX9f9HTfhA3eTN4C1+A75BU/kftqRjr64AXchS21jOxtgmHQP6S+Wr5/Wl8GJJImYAxjOyQAAAAASUVORK5CYII=" class="label_6">
        </div>
        <span>阅读总结</span>
      </div>
    </div>
    <div class="my">
      <div class="save"></div>
      <div class="download"></div>
      <div class="login">
        登录
      </div>
    </div>
  </header>

  <section class="container">
    <SideBar class="sidebar"></SideBar>
    <RouterView />
  </section>
</template>

<style scoped lang="less">
header {
  display: flex;
  width: 100%;
  height: 90px;
  padding: 0 30px;
  justify-content: space-between;
  align-items: center;
  color: #fff;
  position: absolute;
  left: 0;
  top: 0;
  .logo {
    font-family: AlibabaPuHuiTi_3_85_Bold;
    font-size: 24px;
    .title {
      padding-left: 6px;
      vertical-align: top;
    }
  }
  .quick-start {
    width: 250px;
    display: flex;
    justify-content: space-between;
    text-align: center;
    .box {
      width: 45px;
      height: 45px;
      line-height: 45px;
      text-align: center;
      border-radius: 50%;
      img {
        vertical-align: middle;
      }
      &.current {
        background: rgba(255,255,255,.3);
      }
      &:hover {
        background: rgba(255,255,255,.3);
      }
    }
  }
  .my {
    div {
      cursor: pointer;
      &.login {
        width: 32px;
        height: 32px;
        border-radius: 50%;
        line-height: 32px;
        text-align: center;
        background: #C6C4FF;
      }
    }
  }
}

.container {
  display: flex;
  margin-top: 90px;
  padding: 0 7px;
  background: #D7DBFF;
}

.sidebar {
  width: 220px;
  height: calc(100vh - 90px);
  border-radius: 10px 0px 0px 10px;
  background-color: #fff;
}

</style>
