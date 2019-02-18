# **NKUST_Calendar**

將pdf行事曆轉換成json

## Install

```bash
pip3 install -r requirement.txt
```

*Only test in Python3

## Use

1. 先行下載學校[行事曆](https://www.nkust.edu.tw/p/404-1000-4622.php)pdf檔案



```python
from NKUST_Calendar import NKUST_Calendar

print(NKUST_Calendar(file='160007259.pdf',term_year=107).get_json())

```

* term_year 填入這份行事曆的學期年，帶錯會造成周次計算有差

目前支援學校2種格式pdf file 

160007259 / 106188010

cal107-1  / cal107-2 



= U = 



## issues

1. (完成) 測試後目前只支援160007259.pdf/106188010.pdf. 

   cal107-1.pdf 在raw_Calendar_decode 會抓不到events 

   還不確定108之後行事曆依照哪一個版本修改，先暫時支援其中一種

   (2019.02.18 修正 支援2種版本的pdf)



