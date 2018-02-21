---
title: PHPEExcel(支援2007以上讀取)
---
## 使用方法
##讀取寫法
$filename='檔案位置';
$reader= PHPExcel_IOFactory::createReaderForFile($filename);
$reader->setReadDataOnly(true);//設定為只可讀取
$excel = $reader->load($filename);//讀取檔案
$sheet = $excel->getActiveSheet(0);//設定選擇要讀取的excel工作表
$sheet=$excel->getActiveSheet()->toArray(); //轉換成array方式