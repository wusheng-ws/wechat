# wechat
this is my WeChat applet


一、	小程序说明
针对当前中国比较热门的两种考试，公务员考试和考研，本人特地开发了一个刷题小程序，这小程序主要用于刷客观题也即选择题，推出了每日刷题栏目和分类刷题，并且收录了答题人的作答数据，并据此设置了错题集以供下次作答。
二、	数据来源
该小程序数据来源均采用爬虫技术从当前主流的教育网站（中公教育）中获取，根据其每日一题中获取数据，并将其分类整理到该项目的数据库中。部分代码如下图所示，运行该代码即可在数据库中查到对应的题。
 
图2.1 爬虫代码![image](https://user-images.githubusercontent.com/71813070/122633101-596a9480-d109-11eb-9c8e-8e4d7e7935a7.png)


 
图2.2 数据库对应题目![image](https://user-images.githubusercontent.com/71813070/122633098-57a0d100-d109-11eb-8f8c-75aaa7ce7c7d.png)

三、	功能概括
首先当用户首次进入小程序之后，由于小程序后台未记录到该用户的登录数据，所以该用户无法使用小程序所有功能，在其点击功能按钮的时候会弹框提示用户登录。在其正常登录之后，程序可正常使用。 
图3.1刷题页面
![image](https://user-images.githubusercontent.com/71813070/122633096-5374b380-d109-11eb-8386-6615377e745e.png)

	当用户进入刷题页面时，页面如图所示
 
图3.2选择题页面
	程序设置的是每次仅能做四题，做完之后点击查看解析会出现答案解析，并且此时用户作答数据会一并写入数据库中。答案解析中，正确答案用绿色做标记，用户的答案用红色做标记，以便区分。如图3.2-1所示。![image](https://user-images.githubusercontent.com/71813070/122633092-4ce63c00-d109-11eb-8d92-357960f989b1.png)

 
图3.2-2 答案解析
![image](https://user-images.githubusercontent.com/71813070/122633088-49eb4b80-d109-11eb-8cd6-ba92e057f610.png)

在用户点击“立即刷题”按钮的时候，相对应的题就会出现，并且用户可根据“切换”按钮自主选择题库类型，如图3.3所示。
![image](https://user-images.githubusercontent.com/71813070/122633082-4061e380-d109-11eb-8b2a-0bc4d147689b.png)

 
图3.3 切换题库
	如图3.1所示，用户的刷题天数和正确率以及对应的排名均有显示，该数据是结合用户历史数据进行处理的，并与数据库中其他用户作为对比获得的。
	在用户每日刷完对应的习题之后，用户可自主选择以下模块在加强练习。如图3.4所示
  ![image](https://user-images.githubusercontent.com/71813070/122633080-3c35c600-d109-11eb-9c0c-58e7b5bd665a.png)

 
图3.4 分模块刷题
四、	后端
该项目后端采用python flask框架，Flask是一个使用 Python 编写的轻量级 Web 应用程序框架。项目主要代码如下图所示：
![image](https://user-images.githubusercontent.com/71813070/122633077-393ad580-d109-11eb-8a62-23f0206b6713.png)

 
五、	小程序二维码
 ![image](https://user-images.githubusercontent.com/71813070/122633070-2aecb980-d109-11eb-84d5-d1ec83b8ee9f.png)

