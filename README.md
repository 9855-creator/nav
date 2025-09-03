<p align="center">
  <a href="https://nav3.cn/?g">
    <img src="https://gcore.jsdelivr.net/gh/xjh22222228/public@gh-pages/nav/logo.svg" width="130" />
  </a>
  <br />
  <b>发现导航</b>
  <p align="center">一个纯静态、支持SEO、在线编辑的强大导航网站，希望您会喜欢</p>
  <p align="center">内置收录多达 800+ 优质网站， 助您工作、学习和生活</p>
  <p align="center">
    <a href="README_EN.md"><img alt="english" src="https://img.shields.io/static/v1.svg?label=&message=English&style=flat-square&color=ff5000"></a>
    <img src="https://img.shields.io/github/v/release/xjh22222228/nav" />
    <a href="https://github.com/xjh22222228/nav/stargazers"><img src="https://img.shields.io/github/stars/xjh22222228/nav" alt="Stars"/></a>
    <img alt="Angular" src="https://img.shields.io/static/v1.svg?label=&message=Angular&style=flat-square&color=C82B38">
    <img src="https://img.shields.io/github/license/xjh22222228/nav" />
  </p>
</p>



## 设计理念

无数据库、无服务器、零成本一键部署、开箱即用，但又可以像数据库那样操纵数据和保存。

好用、简单、强大。

[谁在使用？](https://official.nav3.cn/?id=3)




#### gh-pages (免费)

1、右上角点击 Fork 当前项目。

2、https://github.com/settings/tokens/new 申请 token, 勾选读写权限, 复制并保存 Token。

3、添加申请的Token https://github.com/你的用户名/nav/settings/secrets/actions/new ，添加申请的 token

4、打开 https://github.com/你的用户名/nav/actions 检查是否已开启 action 自动部署

5、修改项目根目录配置文件 nav.config.yaml 只需要修改仓库地址 gitRepoUrl 字段

6、打开 https://你的用户名.github.io/nav 就能看到一个非常强大的导航网站了。

如果打开 404，请打开 https://github.com/你的用户名/nav/settings/pages 检查分支是否是 gh-pages。

#### Netlify 推荐(免费)

打包路径 `dist/browser`

[https://www.netlify.com/](https://www.netlify.com/)

#### Vercel 推荐(免费)

[https://github.com/apps/vercel](https://github.com/apps/vercel)

#### Cloudflare pages 推荐(免费)

[https://www.cloudflare.com/zh-cn](https://www.cloudflare.com/zh-cn)

## 配置说明

只需要修改根目录 `nav.config.yaml` 以下相关字段
|Fork |自有部署 | 字段 | 说明 |
| --------------------------------------------- | -------- |--- |--- |
|√ | | gitRepoUrl | 填写您的仓库地址 |
|√ | | branch | 部署分支 |
|√ | | imageRepoUrl | 图片仓库, 默认主仓库 `https://github.com/xjh22222228/image?branch=main` |
|√ | √| hashMode | 路由是否 Hash 模式, 如果是部署在 `github pages` 务必设为 true |
|√ | √| email | 用户提交收录通知 |
| | √| password | 自有部署登录密码，`Fork` 用户无需填写 |
| | √| address | 自有部署, 一旦填写认为你是自有部署 |
| | √| mailConfig | 自有部署，用户收录通知邮箱配置 |

## 后台

将路由地址修改为 `system` 即可进入，如: https://www.nav3.cn 修改为 https://www.nav3.cn/system

## 升级

将你的仓库克隆下来执行以下命令

```bash
git pull
git remote add upstream https://gitee.com/xiejiahe/nav.git
git fetch upstream main
git merge upstream/main --allow-unrelated-histories --no-edit
git push

# 如果安装了node只需执行
npm run update
```


## LICENSE

For commercial sites, themes, projects, and applications, keep your source code private/proprietary by purchasing a [Commercial License](https://official.nav3.cn/pricing).

Licensed under the GNU General Public License 3.0 for compatible open source projects and non-commercial use.

Copyright 2024-present xiejiahe
