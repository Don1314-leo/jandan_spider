# jandan_spider
使用selenium爬取煎蛋妹纸图片(Python3)

#### 简介
在脚本中输入煎蛋妹子首页网址'https://jandan.net/ooxx'，
脚本将自动补全网址，并下载煎蛋妹子全站图片。

之所以使用selenium是因为，煎蛋妹子原始图片url不出现在网页原始代码中，但可在chrome开发者工具中的Elements选项卡中查看，而`webdriver.Chrome().get(url_base)`可以轻松获取这些url。


#### 准备工作
测试前请安装好selenium，并在spider_jandan.py当前路径新建img文件夹
- /root
    - /img
    - chromedriver.exe
    - spider_jandan.py
    - README.md
然后执行`python spider_jandan.py`，所有图片将保存在img文件夹中。

鄙人使用如下pakage版本测试通过：
selenium (3.11.0)
requests (2.18.4)

#### 其他信息
此处感谢，抓取煎蛋妹子的创意完全来自kulovecc同学:
https://github.com/kulovecc/jandan_spider
