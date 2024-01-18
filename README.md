# ARL_Asset_Export
[![Python 3.6](https://img.shields.io/badge/python-3.6-green.svg)](https://www.python.org/)

将ARL灯塔中的资产信息详细导出

[ARL灯塔](https://github.com/TophantTechnology/ARL)在任务管理界面可以一键导出详细的资产报告, 但在资产管理页面只能导出域名, url等简单数据.

本工具可以导出某一资产范围下的所有站点, 域名, ip, 和它们的详细信息.

# Usage
1. 修改python脚本中的`url`, `token`, `scope_id`.

2. 执行`python export.py`.

3. 脚本会在工作目录下创建`<scope_id>.xlsx`文件, 包含三个工作表, 分别对应站点, 域名, ip.

# 可导出的内容

## 站点
- URL
- 域名
- ip
- 标题
- 状态码
- 响应头
- 指纹

## 域名
- 域名
- 解析类型
- 记录值

## ip
- ip
- 开放端口
- 端口服务
- 关联域名
- 操作系统
- Geo信息
- ASN信息
