# 东北农业大学考场信息爬取程序

**项目简介：&#x1F449;**


&#x1F625;鉴于东北农业大学考场信息查询网站经常性的会非常缓慢，时不时的还会报错
&#x1F4A1;为了同学们能够稳定快速的查询考场信息
&#x1F4AA;我基于Node.js、axios、cheerio、MongoDB编写了考场信息的爬虫程序

![预览](assets/spider-cmd.gif)

> &#x26A0; Tips：请大家善意测试，最好是在夜深人静的时候....避免占用教务处服务器大量资源影响教务性能


## 要求

  + Node.js v8.9.4
  + MongoDB 数据库已启动，运行端口27017

## 安装 / 开始开发

```bash
  # 安装依赖
  $ npm install

  # 启动开发模式
  $ npm run dev
```

> &#x26A0; Tips：应用将会运行在 [http://localhost:7001/](http://localhost:7001/)

##目录结构

```bash
  # 目录结构
  . spiderExams-neau
  ├── assets       # README.md中用到的图像资源
  ├── src     # 源码
  ├── .gitignore  # git 忽略列表
  └── README.md   # 本说明文件
```

## 运行

```bash
 node ./src/index.js
```

## 设计思路

使用axios.request进行请求，使用cheerio进行解析。

主要内容在index.js中，根据注释阅读代码即可，开发中注意处理爬虫的错误信息，否则会导致程序崩溃，这样的话第二天早上醒来你会发现控制台的命令是红色的...




