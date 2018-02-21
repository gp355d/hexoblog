---
title: PHPEExcel(支援2007以上讀取)
date: 2018-02-21 10:59:14
tags:
---
## 使用方法
##讀取寫法
$filename='檔案位置';
$reader= PHPExcel_IOFactory::createReaderForFile($filename);
$reader->setReadDataOnly(true);//設定為只可讀取
$excel = $reader->load($filename);//讀取檔案
$sheet = $excel->getActiveSheet(0);//設定選擇要讀取的excel工作表
$sheet=$excel->getActiveSheet()->toArray(); //轉換成array方式
## Quick Start

### Create a new post

``` bash
$ hexo new "My New Post"
```

More info: [Writing](https://hexo.io/docs/writing.html)

### Run server

``` bash
$ hexo server
```

More info: [Server](https://hexo.io/docs/server.html)

### Generate static files

``` bash
$ hexo generate
```

More info: [Generating](https://hexo.io/docs/generating.html)

### Deploy to remote sites

``` bash
$ hexo deploy
```

More info: [Deployment](https://hexo.io/docs/deployment.html)

