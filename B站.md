## 收集各个网站的URI
###A站 [http://www.acfun.tv](http://www.acfun.tv "认真你就输了！")


###B站 [http://www.bilibili.com](http://www.bilibili.com "哔哩哔哩弹幕网站")
#### 视频播放页面（http://www.bilibili.com/video/av4303756/）
* 获取cid<br>http://www.bilibili.com/video/av4303756/<br><script type='text/javascript'>EmbedPlayer('player', "http://static.hdslb.com/play.swf", "cid=6962886&aid=4303756");</script>
* 获取评论 <br>http://api.bilibili.com/x/reply?oid=4303756&type=1&pn=2<br>
* 观看次数 <br>http://interface.bilibili.com/count?key=5febfb9006283a2e07e6f711&aid=4303756&mid=3792124<br> 111;$('#dianji').html('105817');$('#stow_count').html('4416');$('#v_ctimes').html(4750);$('.v_ctimes').html(4750);$('#dm_count').html(2144);$('.dm_count').html(2144);
* 获取视频标签<br>http://www.bilibili.com/api_proxy?app=tag&action=/tags/archive_list&aid=4303756&nomid=1
* 当前用户的权限信息<br>http://interface.bilibili.com/player?id=cid:6962886&aid=4303756<br>
* 弹幕信息<br>http://comment.bilibili.com/6962886.xml

#### 一级视频分类页面（n.json，n表示某种分类，对应typeid，n-time.json，time可以是week和3-day，表示某种分类下的近一周和近三天的热门视频）
* 新动态，返回视频编号<br>http://www.bilibili.com/index/ding-count.json
* 推荐的视频（轮播图）<br>http://www.bilibili.com/index/slideshow/4.json
* 获取视频<br>http://www.bilibili.com/index/catalogy/5-recommend.json
* 热门视频统计<br>http://www.bilibili.com/index/catalogy/24-week.json
* 获取视频<br>http://www.bilibili.com/index/ding/24.json
* 未知<br>http://www.bilibili.com/plus/widget/ajaxGetCaptchaKey.php<br>f48d75e4283aa794d0e9455f4387be22
* 返回视频信息的数据格式<br>aid:4305518<br>typeid:27<br>title:"[排行向]二次元红毛美少女排行"<br>subtitle:""<br>play:96251<br>review:816<br>video_review:13036<br>favorites:3378<br>mid:113711<br>author:"疾風醬"<br>description:"自制 720P 红发少女热情如火!!曲+图包:http://pan.baidu.com/s/1nvepjdB"<br>create:"2016-04-08 09:41"<br>pic:"http://i2.hdslb.com/bfs/archive/4aaf207060b8fa1fa021e90d77dc856b9dc18abe.jpg_320x200.jpg"<br>credit:0<br>coins:3739<br>duration:"12:18"

#### 用户信息（http://space.bilibili.com/6348263）
* 用户信息<br>http://space.bilibili.com/ajax/member/GetInfo?mid=6348263<br>{"status":true,"data":{"mid":"6348263","name":"\u6d6e\u7a7a\u75c7","approve":false,"sex":"\u7537","rank":"10000","face":"http:\/\/i0.hdslb.com\/bfs\/face\/d690ef1a861b9be8b8b669279af4d3b8053e7380.gif","coins":0,"DisplayRank":"10000","regtime":1411786766,"spacesta":0,"birthday":"2016-01-01","place":"\u5b89\u5fbd\u7701 \u829c\u6e56\u5e02","description":"","article":0,"attentions":[4931993,4400955,1332697,4573095,7287761,221648,375375,3020100,296515,826317,1699331,458203,1950746,10579922,11709157,912725,2788680,2990632,2486204,4604408,6857104,5860126,19456751,7714,883968,212230,8578857,11417691,20646254,14558631,1532165,433351],"fans":9472,"friend":32,"attention":32,"sign":"\u597d\u70e6\u554a\uff01\u4e0a\u65b0\u5408\u96c6\uff0c\u5e0c\u671b\u53ef\u4ee5\u9759\u4e0b\u5fc3\u6765\u770b\u5b8c","level_info":{"current_level":4,"current_min":4500,"current_exp":6157,"next_exp":10800},"pendant":{"pid":0,"name":"","image":"","expire":0},"nameplate":{"nid":7,"name":"\u89c1\u4e60\u642c\u8fd0\u5de5","image":"http:\/\/i2.hdslb.com\/group1\/M00\/CC\/B0\/oYYBAFbBmeSAOWZnAAAFvEbG7S4702.png"},"toutu":"group1\/M00\/F8\/6F\/oYYBAFalnNSAdVoSAABmUQZp6v8341.jpg","theme":"default","theme_preview":"","im9_sign":"b334b0f943e99dd535123165f06dc6ca"}}
* 得到标签<br>http://space.bilibili.com/ajax/member/getTags?mids=6348263
* 置顶视频<br>http://space.bilibili.com/ajax/top/showTop?mid=6348263
* 他关注的人<br>http://space.bilibili.com/ajax/friend/GetAttentionList?mid=6348263&pag=1
* 他的粉丝<br>http://space.bilibili.com/ajax/friend/GetFansList?mid=6348263&page=1
* 订阅<br>http://space.bilibili.com/ajax/Bangumi/getList?mid=6348263
* 兴趣圈<br>http://www.im9.com/api/query.my.community.list.do?mid=6348263&data_type=2&page_size=12&page_no=1&sign=b334b0f943e99dd535123165f06dc6ca&space_callback=space_callback&type=jsonp&ts=1460273788
