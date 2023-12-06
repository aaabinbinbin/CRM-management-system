# CRM

CRM相关概念参考：

- https://baike.baidu.com/item/%E5%AE%A2%E6%88%B7%E5%85%B3%E7%B3%BB%E7%AE%A1%E7%90%86/254554
- https://wiki.mbalib.com/wiki/%E5%AE%A2%E6%88%B7%E5%85%B3%E7%B3%BB%E7%AE%A1%E7%90%86
- https://www.oracle.com/cn/cx/what-is-crm/#link16

CRM系统核心对象是客户、线索、联系人、业务机会，这四者之间的对应关系如下：

![co-relation](.\public\co-relation.png)

- **客户**
  - 发生交易行为的主体。
  - 在不同的行业以及不同的环节中，客户所对应的对象不同，可以是某个组织也可以是个人，并且能够具有一定的组织架构。
- **线索（潜在客户）**
  - 是可能会发生交易的对象或者对象资料。
  - 线索可以通过业务机会转换为客户，而线索转化为客户的过程就是线索的转换过程。
- **联系人**
  - 与企业交互的主体，对交易有影响的人，也可以是业务对接人。
  - 联系人可能就是客户本身，也可能是其他（比如某企业准备采购一批硬盘，客户就是企业这个组织，但是联系人可能是采购员、也可能是财务专员，与企业组织结构有关）。
- **业务机会（商机）**
  - 产生交易的机会。
  - 业务机会来源于客户，一个客户可能有多次交易，业务机会就是每一次客户想要购买某个产品或服务的意向，也是完成销售业绩的开端。

# 项目简介

`crmsys`是一款创新型客户关系管理软件，专为现代企业的增长和竞争优势而设计。它提供了一套全面的工具和功能，使企业能够深入了解客户需求、提供卓越的服务、拓展市场份额，以及实现高效的销售和营销策略。

本系统适用各类行业，主要针对中小型销售/售后服务团队，该系统支持客户资料自定义配置、查询。

**主要功能和特点：**

- **360度客户视图：** 通过集成各个渠道的数据，为企业提供全面的客户视图，帮助他们更好地了解客户的需求和行为。
- **销售自动化：** 自动化销售流程，包括线索跟进、销售机会管理、报价和订单处理，提高销售效率，减少错误。
- **客户服务和支持：** 提供多渠道客户服务和支持，包括在线聊天、电子邮件和电话支持，确保客户满意度和忠诚度。
- **移动应用支持：** 提供移动应用程序，使销售团队和客户支持人员能够在任何地方访问关键数据和工具。
- **弹性和可扩展性：** 基于微服务架构，系统具有强大的弹性和可扩展性，可以适应不断变化的业务需求。
- **智能分析和洞察：** 利用先进的数据分析和机器学习算法，系统可以为企业提供深刻的市场洞察，帮助他们优化营销策略和产品开发。

**业务价值：**

- **客户增长：** 通过更好地了解客户需求和提供卓越的服务，企业可以吸引更多客户，实现持续的增长。
- **销售扩张：** 自动化销售流程和智能洞察帮助销售团队更快地关闭交易，扩展市场份额。
- **数据驱动决策：** 数据分析和智能洞察使企业能够制定更明智的决策，优化资源分配，并预测市场趋势。
- **客户满意度提高：** 通过提供更好的客户服务和支持，CRM系统可以提高客户满意度，增强客户忠诚度。

# 前端技术栈

## 核心技术栈

| 技术           | 说明             | 版本                                                         | 备注                                 |
| -------------- | ---------------- | ------------------------------------------------------------ | ------------------------------------ |
| `Vue`          | 前端框架         | `v3.x`                                                       | https://v3.vuejs.org/                |
| `Vue-Router`   | 路由框架         | `v4.x`                                                       | https://next.router.vuejs.org/       |
| `Pinia`        | 全局状态管理框架 | `v2.x`                                                       | https://pinia.vuejs.org/             |
| `Axios`        | HTTP中间件       | [`v0.27.2`](https://github.com/axios/axios/releases/tag/v0.27.2) | https://github.com/axios/axios       |
| `Element-Plus` | 前端`UI`框架     | `latest`                                                     | https://element-plus.gitee.io/zh-CN/ |

## 扩展技术栈

| 技术                 | 说明                    | 版本     | 备注                                                         |
| -------------------- | ----------------------- | -------- | ------------------------------------------------------------ |
| `Avue`               | 基于`ElementUI`二次封装 | `v3.1.4` | https://v3.avuejs.com/                                       |
| `V-Charts`           | 基于`Echarts`的图表框架 | latest   | https://v-charts.js.org/                                     |
| `AJ-Captcha`         | 验证码插件              | 1.3.0    | https://ajcaptcha.beliefteam.cn/captcha-doc/                 |
| `SheetJS`            | 电子表格插件            | 0.19.2   | https://docs.sheetjs.com/docs/<br>https://docs.sheetjs.com/docs/demos/frontend/vue |
| `vue-plugin-hiprint` | 打印插件                | 0.0.48   | https://gitee.com/CcSimple/vue-plugin-hiprint                |
| `wangEditor`         | 富文本编辑器            | v5       | https://www.wangeditor.com/v5/                               |

# `IDE`设置要求

你可以直接使用`WebStorm`、`HBuilderX` 或 `IDEA`作为开发`IDE`，也可以使用`VSC`。

如果你要使用`VSC`可以使用下面的搭配：

[`VSCode`](https://code.visualstudio.com/) + [`Volar`](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (需要禁用`Vetur`) + [`TypeScript Vue Plugin (Volar)`](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin)。

# 自定配置选项

详情请参阅：[`Vite Configuration Reference`](https://vitejs.dev/config/).

# 项目设置

安装依赖，使用下面的命令行安装：

```sh
npm install
```

### 开发时：编译并以热加载的方式启动项目

```sh
npm run dev
```

### 发布时：编译并压缩代码

```sh
npm run build
```

### 使用[`ESLint`](https://eslint.org/)检查代码

```sh
npm run lint
```

# 目录结构说明

下面目录或文件为有效资源，其他目录或文件不要提交到服务端：

- public：存放开放资源，比如比较大的图片文件或站点图标
- `src`：存放资源和源码的目录，注意`.vue`文件文件名大写字母开头
  - `src/apis`：存放网络对接`api`接口实现
  - `src/assets`：小资源文件可以放图标文件或全局样式表
  - `src/components`：存放公用组件
  - `src/plugins`：存放自定义插件封装
  - `src/router`：路由配置文件目录
  - `src/stores`：状态管理文件目录
  - `src/views`：存放页面目录
  - `src/App.vue`：程序入口`vue`文件
  - `src/main.js`：程序入口挂载以及插件装配文件
- .`env.XXX`：为环境变量文件
- `.eslintrc.cjs`：为`eslint`配置文件
- `.gitignore`：忽略配置文件
- `.prettierrc.json`: 代码美化配置文件
- `index.html`：程序入口页面
- `package.json`：第三方`JS`库管理配置文件
- `README.md`：项目自述文件
- `vite.config.js`：`Vite`构建工具配置文件
- `start.sh`：`Linux`下面的启动脚本

