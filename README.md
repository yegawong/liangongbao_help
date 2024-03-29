# liangongbao_help
## 有任何问题，可加Q群交流: 644738320
## 学习交流如有侵权联系删除

----------------------------

# 默认无题库，题库去群里求大佬们,一定一定放好题库在答题，可以用更改'config/LgbConfig.py'中 'ONLY_QUERYINFO = True' 先不答题测试程序是否正常运行
----------------------------

# 项目初衷让人人学会安全生产，学习交流技术，请勿商用软件，请勿打赏任何人，发现后立即停止更新项目。
动动你的小手帮助群里的小白，人多力量大

----------------------------

## 功能
- 支持使用接口答题
- 使用接口重连功能
- 支持浏览器自动化答题
- *支持OCR识别手机题目手动答题*
- 多题库匹配
- Excel题库
- TXT题库
- 安全法文章匹配提醒机制
- 支持题目匹配失败时手动作答
- 错题汇总共同交流
- 随机答题数目或者全部默认作答
- 用户积分，抽奖次数查询等
- 自动抽奖功能
- 2023年微信登录答题
- 微信持久化登录
- 增加cookie处理
- 增加详细日志记录
- 增加异常处理机制
- 增加题库选择优先级

## 未来展望
- 增加单元测试，MOCK接口等

# Install
```shell
  #2023 python 3.7+
  pip install -r requirements.txt

# 2023年需要得无影响
# 由于版本过高，无法安装onnxruntime, 创建虚拟环境或python版本降级
# 可以运行的办法：python>=3.10不适用可视化功能，直接注释掉requirements_2022.txt中的ddddocr, 如 #ddddocr
```
# run
运行前去群里向大佬们求下载题库，解压得到question_bank文件夹，将文件夹放在项目根目录下，目录结构：

```shell
./question_bank/xx.txt
./question_bank/xx.xls
...
```

学习交流为主，其他勿扰
按需更改 config/LgbConfig.py 配置即可
正常情况下，是不需要手动输入答案的，一直有新的running跳动，每题默认延迟2-5s
需要手动答题的时候，只需要输入正确选项'A,B,C,D'，输入不在选项中时会提示重新输入,输入为空同理
用答过题的账号尝试可视化登录，也挺好玩~

```shell
python main.py -i
```
# 题库找不到答案，手动输入例子如图
![image](手动输入例子.png)


# usage
```shell
usage: main.py [-h] [-i] [-v] [-a] [-w] [-g]

链工宝让平凡的人懂得安全生产

options:
  -h, --help            show this help message and exit
  -i, --interface_call  2023使用手机APP接口POST/GET运行
  -v, --visualization   2022使用浏览器可视化运行
  -a, --adb_ocr         2022使用ADB工具连接手机运行
  -w, --webpc           2023使用Wechat登录网页版运行
  -g, --get_wechat_token_mul
                        2023获取Wechat登录多个token
```