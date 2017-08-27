# pynew
pynew是一个精简的新闻搜索工具，是国科大信息检索课程作业之一。    
线下爬取各个新闻网站的内容，线上通过简单的编辑距离和倒排索引等方式实现搜索。
## 环境要求
 - python 2.7
 - scrapy 1.0.3
 - jinja2 2.8
 - jieba  0.38
 - numpy  1.8.2
 - scipy  0.13.3
 - sklearn 0.0    

## 快速开始
 - git clone 
 - sudo pip install -r requests.txt
 - cd pynew/spider
 - scrapy crawl sinaspider      爬取新浪新闻
 - scrapy crawl netesespider    爬取网易新闻
 - scrapy crawl tencentspider    爬取腾讯新闻
 - cd pynew/UI
 - python server.py             运行服务端程序
 - 打开浏览器输入http://localhost:5000    

## 输出
-[+]data    
 | [+]sina    
 | | [+]comments         所有评论    
 | | [+]html             html页面    
 | | [+]interest_news    我们感兴趣的信息    
 | [+]tencent    
 | | [+]comments    
 | | [+]html    
 | | [+]interest_news    
 | [+]netese    
 | | [+]comments    
 | | [+]html    
 | | [+]interest_news    

## 我们感兴趣的信息定义
 - ID             新闻ID
 - URL            新闻URL
 - Time           新闻时间
 - Keyword        新闻关键字
 - Source         新闻来源
 - Channel        新闻频道
 - Total          新闻评论总数
 - Title          新闻标题
 - Artical        新闻主体
 - Comment        评论内容
 - Html           新闻页面

