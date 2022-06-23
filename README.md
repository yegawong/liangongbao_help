# liangongbao_help

## 功能
- #####  支持使用接口答题
- #####  使用接口重连功能
- #####  支持浏览器自动化答题
- #####  *支持OCR识别手机题目手动答题*
- #####  多题库匹配
- #####  Excel题库
- #####  TXT题库
- #####  安全法文章匹配提醒机制
- #####  支持题目匹配失败时手动作答
- #####  错题手机共同交流

## 未来展望
- #####  增加详细日志记录
- #####  增加异常处理机制
- #####  增加cookie处理
- #####  邮件通知
- #####  docker定时运行等
- #####  增加单元测试，MOCK接口等


# run
```shell
按需更改 LgbConfig.py 配置即可

pip install -r requirements.txt
python main.py

```

# usage
```shell

  usage: main.py [-h] [-i] [-v] [-a]

  链工宝让平凡的人懂得安全生产

  optional arguments:
    -h, --help            show this help message and exit
    -i, --interface_call  使用接口POST/GET运行
    -v, --visualization   使用浏览器可视化运行
    -a, --adb_ocr         使用ADB工具连接手机运行
```


# 有任何问题，可加Q群交流: 644738320
## 学习交流如有侵权请联系我删除