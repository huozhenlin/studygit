# 基于互联网大数据的事件智能抓取和画像

## 注意事项

- **背景**
    
    随着互联网大数据的发展，各种大数据的分析对各行业都产生了不同程度的影响。网站数据、社交媒体数据等是互联网大数据的重要组成部分。对于民航业领域，社会事件的发生，会很大程度影响旅客的出行需求变化，从而影响航空公司飞机运力投放、航班编排、票价策略调整等，对互联网事件的准确抓取和分析能够帮助航空公司更好的服务市场、服务旅客、提升收益等。

- **开发语言**

    <font face="微软雅黑" color="blue"size=3>Python</font>(数据挖掘和分析)<br>
    <font face="微软雅黑"color="blue"size=3>Javascript</font>(用于数据可视化)<br>
    <font face="微软雅黑"color="blue"size=3>PHP</font>(后台语言)

- **演示**

    ![Sample Video](https://gitlab.com/gitlab-org/gitlab-ce/raw/master/doc/user/img/markdown_video.mp4)

-  **数据可视化地址**

    <http://url.com>
   
## 软件使用前准备工作

- **python版本号**(v2.7)

- **自动化测试驱动**(选其一，根据实际情况修改代码中的驱动调用即可)
        
        1.Chrome
        2.PhantomJS


>   例子:

    ```python
    driver=webdriver.PhantomJS
    ```

- **主要使用到的框架，模块，请前往对应官网下载**

| 模块 | 用途 |
| -------- | -------- |
| requests   | 进行网络请求   |
| BeautifulSoup   | 将网页源代码生成树状结构，便于抽取想要的内容   |
| selenium        |      自动化测试工具，用于请求网页中使用ajax技术调用的数据|
| re        |     通过正则表达式匹配想要获取的内容|
| echart|用于数据可视化|
| pyltp|自然语言处理，分词用到|
| pandas|数据处理|
| Simhash|利用simhash，海明距离对重复事件去重|
| ...|...|

>   <font color="red"">注意:</font>
    
分词模型采用本地化分词，[点击下载](baidu.com),导入方式如下

```python
from pyltp import Segmentor
segmentor = Segmentor()
segmentor.load(r'C:\Users\hzl\PycharmProjects\untitled\chinasoftbei\analyse\ltp_data\cws.model')  # 分句模型
```

## 特性和功能
1. **事件去重**
2. **准确的关键字提取**
3. **事件属性自动化提取**(包含时间，地点，影响人群，影响区域，主办方级别)
4. **简洁明了的可视化界面**
5. **丰富的事件来源**(爬取了发布事件的主流网站)

## 软件安装及使用

## 未来计划

## 遵循协议















