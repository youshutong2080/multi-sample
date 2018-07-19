<template>
  <div class="home">
    <div class="header-con">
      <div class="header-logo">
        <img src="data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0idXRmLTgiPz4NCjwhLS0gR2VuZXJhdG9yOiBBZG9iZSBJbGx1c3RyYXRvciAxOS4wLjAsIFNWRyBFeHBvcnQgUGx1Zy1JbiAuIFNWRyBWZXJzaW9uOiA2LjAwIEJ1aWxkIDApICAtLT4NCjxzdmcgdmVyc2lvbj0iMS4xIiBpZD0i5Zu+5bGCXzEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHg9IjBweCIgeT0iMHB4Ig0KCSB2aWV3Qm94PSIwIDAgNjQgNjQiIHN0eWxlPSJlbmFibGUtYmFja2dyb3VuZDpuZXcgMCAwIDY0IDY0OyIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSI+DQo8c3R5bGUgdHlwZT0idGV4dC9jc3MiPg0KCS5zdDB7ZmlsbDojRkZGRkZGO30NCgkuc3Qxe2ZpbGw6IzJEOENFRjt9DQoJLnN0MntmaWxsOiMyREY1QkU7fQ0KPC9zdHlsZT4NCjxwYXRoIGNsYXNzPSJzdDAiIGQ9Ik01MywwSDExQzQuOSwwLDAsNC45LDAsMTF2NTNoNTNjNi4xLDAsMTEtNC45LDExLTExVjExQzY0LDQuOSw1OS4xLDAsNTMsMHoiLz4NCjxwYXRoIGNsYXNzPSJzdDEiIGQ9Ik0yNC40LDE1LjFjLTEsMC0xLjksMC44LTEuOSwxLjl2NC41YzAsMSwwLjgsMS45LDEuOSwxLjloNC4zdjI4LjRoOC4yYzAsMCwwLDAsMCwwVjIzLjNoMTIuMw0KCWMxLDAsMS45LTAuOCwxLjktMS45di02LjRIMjQuNHoiLz4NCjxwYXRoIGNsYXNzPSJzdDIiIGQ9Ik0xOC4xLDIzLjNoLTQuNWMtMSwwLTEuOS0wLjgtMS45LTEuOXYtNi4zaDYuM2MxLDAsMS45LDAuOCwxLjksMS45djQuNUMyMCwyMi41LDE5LjEsMjMuMywxOC4xLDIzLjN6Ii8+DQo8L3N2Zz4NCg==" alt="">
        <img class="header-logo-line" src="data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz4NCjxzdmcgd2lkdGg9IjRweCIgaGVpZ2h0PSI2NHB4IiB2aWV3Qm94PSIwIDAgNCA2NCIgdmVyc2lvbj0iMS4xIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHhtbG5zOnhsaW5rPSJodHRwOi8vd3d3LnczLm9yZy8xOTk5L3hsaW5rIj4NCiAgICA8IS0tIEdlbmVyYXRvcjogU2tldGNoIDQxLjIgKDM1Mzk3KSAtIGh0dHA6Ly93d3cuYm9oZW1pYW5jb2RpbmcuY29tL3NrZXRjaCAtLT4NCiAgICA8dGl0bGU+bGluZTwvdGl0bGU+DQogICAgPGRlc2M+Q3JlYXRlZCB3aXRoIFNrZXRjaC48L2Rlc2M+DQogICAgPGRlZnM+PC9kZWZzPg0KICAgIDxnIGlkPSJQYWdlLTEiIHN0cm9rZT0ibm9uZSIgc3Ryb2tlLXdpZHRoPSIxIiBmaWxsPSJub25lIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIG9wYWNpdHk9IjAuNSI+DQogICAgICAgIDxnIGlkPSLlupTnlKjmpoLop4giIHRyYW5zZm9ybT0idHJhbnNsYXRlKC0xMjguMDAwMDAwLCAtNDAuMDAwMDAwKSI+DQogICAgICAgICAgICA8ZyBpZD0ibG9nbyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoNDAuMDAwMDAwLCAzMC4wMDAwMDApIj4NCiAgICAgICAgICAgICAgICA8ZyBpZD0ibGluZSIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoODguMDAwMDAwLCAxMC4wMDAwMDApIj4NCiAgICAgICAgICAgICAgICAgICAgPHBhdGggZD0iTTIsMCBMMiwyMCIgaWQ9IkxpbmUiIHN0cm9rZT0iI0ZGRkZGRiIgc3Ryb2tlLXdpZHRoPSIyIj48L3BhdGg+DQogICAgICAgICAgICAgICAgICAgIDxwYXRoIGQ9Ik0yLDQ0IEwyLDY0IiBpZD0iTGluZS1Db3B5IiBzdHJva2U9IiNGRkZGRkYiIHN0cm9rZS13aWR0aD0iMiI+PC9wYXRoPg0KICAgICAgICAgICAgICAgICAgICA8Y2lyY2xlIGlkPSJPdmFsIiBmaWxsPSIjRkZGRkZGIiBjeD0iMiIgY3k9IjMyIiByPSIyIj48L2NpcmNsZT4NCiAgICAgICAgICAgICAgICA8L2c+DQogICAgICAgICAgICA8L2c+DQogICAgICAgIDwvZz4NCiAgICA8L2c+DQo8L3N2Zz4=" alt="">
        <div class="header-logo-title">
          <h3>配置管理</h3>
          <h4>Seasungame SCM</h4>
        </div>
      </div>
      <div class="header-aside">
        <div class="header-aside-phone"></div>
        <div class="header-aside-window">
          <Tooltip content="进入全屏" placement="bottom">
            <font-awesome-icon :icon="['fas', 'expand-arrows-alt']"></font-awesome-icon>
          </Tooltip>
        </div>
        <div class="header-aside-setting">
          <Tooltip content="全局设置" placement="bottom">
            <font-awesome-icon :icon="['fas', 'cogs']"></font-awesome-icon>
          </Tooltip>
        </div>
        <div class="header-aside-bell">
          <Tooltip content="您有3条未读消息" placement="bottom">
            <Badge dot>
              <font-awesome-icon icon="bell"></font-awesome-icon>
            </Badge>
          </Tooltip>
        </div>
        <div class="header-aside-dropdown-menu">
          <Dropdown placement="bottom-end">
            <font-awesome-icon icon="user-circle"></font-awesome-icon>
            <Icon type="ios-arrow-down"></Icon>
            <DropdownMenu slot="list">
              <DropdownItem name="ownSpace">
                <font-awesome-icon :icon="['fas', 'user-shield']"></font-awesome-icon>
                <span>个人中心</span>
              </DropdownItem>
              <DropdownItem name="loginOut">
                <font-awesome-icon :icon="['fas', 'sign-out-alt']"></font-awesome-icon>
                <span>退出登陆</span>
              </DropdownItem>
            </DropdownMenu>
          </Dropdown>
        </div>
      </div>
      <div class="header-aside header-aside-small">
        <Dropdown placement="bottom-end">
          <font-awesome-icon :icon="['fas', 'ellipsis-v']"></font-awesome-icon>
          <DropdownMenu slot="list">
            <DropdownItem name="fullScreen">
              <font-awesome-icon :icon="['fas', 'expand-arrows-alt']"></font-awesome-icon> 进入全屏
            </DropdownItem>
            <DropdownItem name="pageSetting">
              <font-awesome-icon :icon="['fas', 'cogs']"></font-awesome-icon> 全局设置
            </DropdownItem>
            <DropdownItem name="message">
              <font-awesome-icon icon="bell"></font-awesome-icon> 消息中心
            </DropdownItem>
          </DropdownMenu>
        </Dropdown>
      </div>
      <div class="header-items" style="margin-left: 15px;">
        <a><font-awesome-icon :icon="['fas', 'coins']"></font-awesome-icon> <span>资源管理</span></a>
        <a><font-awesome-icon :icon="['fas', 'tasks']"></font-awesome-icon> <span>工单系统</span></a>
        <a><font-awesome-icon :icon="['fas', 'user-cog']"></font-awesome-icon> <span>用户系统</span></a>
      </div>
      <div class="header-items header-items-small" style="margin: 0 15px;">
        <a style="line-height: 20px; top: 3px;" @click="toggleCollapsed"><font-awesome-icon :icon="['fas', 'braille']"></font-awesome-icon></a>
        <a style="line-height: 20px; top: 3px;"><font-awesome-icon :icon="['fas', 'coins']"></font-awesome-icon></a>
        <a style="line-height: 20px; top: 3px;"><font-awesome-icon :icon="['fas', 'tasks']"></font-awesome-icon></a>
        <a style="line-height: 20px; top: 3px;"><font-awesome-icon :icon="['fas', 'user-cog']"></font-awesome-icon></a>
      </div>
    </div>
    <div class="layout">
      <Layout style="height: 100%;">
        <Sider ref="sider" class="layout-sider-con" breakpoint="md" :theme="!isCollapsed ? 'light' : 'dark'" :width="!isCollapsed ? 200 : 60" :collapsed-width="60" v-model="isCollapsed">
          <sider-no-collapsed v-if="!isCollapsed"></sider-no-collapsed>
          <sider-collapsed v-else ></sider-collapsed>
        </Sider>
        <Layout :style="{padding: '0 24px 24px'}">
          <Breadcrumb :style="{margin: '24px 0'}">
            <BreadcrumbItem>Home</BreadcrumbItem>
            <BreadcrumbItem>Components</BreadcrumbItem>
            <BreadcrumbItem>Layout</BreadcrumbItem>
          </Breadcrumb>
          <Content :style="{padding: '24px', minHeight: '280px', background: '#fff'}">
            Content
          </Content>
        </Layout>
      </Layout>
    </div>
  </div>
</template>

<script>
import siderNoCollapsed from './components/sider-no-collapsed'
import siderCollapsed from './components/sider-collapsed'

export default {
  name: 'home',
  components: {
    siderNoCollapsed,
    siderCollapsed
  },
  data () {
    return {
      isCollapsed: false
    }
  },
  methods: {
    toggleCollapsed () {
      this.isCollapsed = !this.isCollapsed
      console.log(this.isCollapsed)
    }
  }
}
</script>

<style lang="less" scoped>
@import '../assets/less/home.less';
</style>
