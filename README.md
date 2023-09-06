## 爬虫爬取福州大学的通知、文件系统

1.任务：爬取福大通知、文件系统

> 爬取福州大学通知、文件系统（https://info22.fzu.edu.cn/lm_list.jsp?wbtreeid=1460 )

包含发布时间，作者，标题以及正文。

可自动翻页（爬虫可以自动对后续页面进行爬取，而不需要我们指定第几页）

范围：2020年1月1号 - 2021年9月1号（不要爬太多了）。

2.使用的技术栈:Java的Jsoup库
3.主要解决的问题：
因为网站需要登录，所以通过发送post请求，然后就会返回cookie或者token，获取cookie并加入下一个请求的请求头。