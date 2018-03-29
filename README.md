## 背景

网易 lordofpomelo 项目年久失修，依赖库的版本存在各种问题，导致无法按照官方文档正常运行。本库是修复了系列问题可运行版本。

## 主要修改
1. mysql、generic-pool 两个库使用最新版本且固定大版本号
2. 修复 express 版本与其依赖的 mime 库版本不兼容的情况
3. 修正因依赖库升级带来 API 的变动问题
4. 修正 web-server 下 component 打包输出文件中的错误

## 运行指南
1. 运行根目录的 `npm-install.sh`，等待依赖安装完毕
2. 使用 `game-server/config/scheme/Pomelo.sql` 创建项目数据库
3. 修改 `shared/config/mysql.json` 数据库连接配置
4. 分别开启游戏服务器与 Web 服务器
    1. `pomelo start -e development`
    2. `node app`
5. 浏览器打开 `http://127.0.0.1:3001/`，开始体验吧

## 附录
1. [NetEase/lordofpomelo](https://github.com/NetEase/lordofpomelo)
2. [lordofpomelo 安装指引](https://github.com/NetEase/pomelo/wiki/Installation-guide-of-lordofpomelo)
