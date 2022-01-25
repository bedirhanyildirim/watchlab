<template>
  <div id="app">
    <el-container>
      <el-header>
        <el-container direction="horizontal">
          <div class="logo">
            WATCH/LAB
          </div>
          <el-menu
            mode="horizontal"
            background-color="#ffffff"
            text-color="#000000"
            default-active="1"
            active-text-color="#000000"
          >
            <el-menu-item index="1">About Us</el-menu-item>
            <el-menu-item index="2">Brand</el-menu-item>
            <el-menu-item index="3">Projects</el-menu-item>
            <el-menu-item index="4">Magazine</el-menu-item>
            <el-menu-item index="5">Press</el-menu-item>
            <el-menu-item index="6">Contacts</el-menu-item>
          </el-menu>
          <div class="search">
            <el-input
              suffix-icon="el-icon-search"
              type="text"
            ></el-input>
          </div>
        </el-container>
      </el-header>
      <el-main>
        <span>main</span>
      </el-main>
      <el-footer>Footer</el-footer>
    </el-container>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style lang="scss">
#app {
  font-family: Merriweather;

  .el-header {
    padding: 0;
    width: 100%;

    .el-container {
      padding: 0;
      width: 100%;
      font-family: Montserrat;
      justify-content: space-between;
    }

    .logo {
      height: 100%;
      padding: 16px;
      display: flex;
      color: #ffffff;
      font-size: 24px;
      font-weight: bold;
      letter-spacing: 4px;
      align-items: center;
      justify-content: center;
      background-color: #D0C5B6;
    }

    .el-menu {
      border: none;
      font-weight: normal;

      .el-menu-item {
        margin: 0 20px;
        padding: 0 20px;
        font-size: 14px;

        &.is-active {
          border-color: #D0C5B6!important;
        }

        &:hover {
          background-color: inherit!important;
        }
      }
    }

    .search {
      display: flex;
      align-items: center;
      justify-content: center;
      border: none;
      padding: 0 20px;

      .el-input.el-input--suffix {
        border: none;
        color: #000000;

        .el-input__inner {
          border: none;
          border-radius: 0;
          border-bottom: 1px solid #000000;
        }
      }
      .el-input__suffix {
        color: #000000;
      }
    }
  }
}
</style>
