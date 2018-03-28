## 背景

网易 lordofpomelo 项目年久失修，依赖库的版本错乱，无法正常运行。这个是修复了系列问题可运行版本。

## 主要修改
1. mysql、generic-pool 两个库使用最新版本且固定大版本号
2. 修正因依赖库升级带来 API 的变动问题
3. 修正 web-server 下 component 打包输出文件存在错误的问题

## 附录
1. [NetEase/lordofpomelo](https://github.com/NetEase/lordofpomelo)
2. [lordofpomelo 安装指引](https://github.com/NetEase/pomelo/wiki/Installation-guide-of-lordofpomelo)
