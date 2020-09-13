---
title: My Hexo Blog
date: 2020-07-07 21:22:21
tags:
- 随记
categories:

thumbnail: https://s1.ax1x.com/2020/08/20/dJabfP.jpg
top: 1
---
我是xzMhehe，一名Java开发者，技术一般，经历平平，但是也一直渴望进步，同时也努力活着，为了人生不留遗憾，也希望能够一直做着自己喜欢的事情，得闲时分享心得、分享一些浅薄的经验，等以后老得不能再老了，就说故事已经讲完了,不去奢求圆满。
相信浏览这段话的你也知道，学习是一件极其枯燥而无聊的过程，甚至有时候显得很无助，我也想告诉你，成长就是这样一件残酷的事情，任何成功都不是一蹴而就，需要坚持、需要付出、需要你的毅力，短期可能看不到收获，因为破茧成蝶所耗费的时间不是一天



## 关于Blog

> 本站历史(Hexo 搭建巧了)
<p>博客从<ahref="http://localhost:4000/2019/12/29/%E8%A7%86%E5%9B%BE%E7%9A%84%E6%93%8D%E4%BD%9C"><strong>2019.8.11</strong></a>至今已经运行<span id="htmer_time" style="color: #90CAF9; font-weight: bold;"></span></p>

## 起步

>📝记录从初识到熟悉的过程

## 再次起步

- 博客园    https://www.cnblogs.com/mzdljgz/    
- CSDN  https://blog.csdn.net/weixin_43874301
- 简书  https://www.jianshu.com/u/a22e10515f17
- 知乎  https://www.zhihu.com/people/jing-qing-qiu-52
- 掘金  https://juejin.im/user/131597127652312
- 公众号 ThePalmJava

为什么把博客园放在首位, 因为我第一次接触的就是博客园. 当时也发文章, 主要是自己遇到的问题以及解决方案. 不查历史记录的话, 已经忘记了什么时候开始写了（查了下posted @ 2018-11-26 21:08 马总丢了紧箍咒 阅读(71) 评论(0) 推荐(0) 编辑）. 立个flag 无论是处在研发岗位还是管理岗位要一直写下去.

## 至今
现在还是在校生, 继续技术探索. 继续以弘扬互联网精神为己任，自己有意创建技术社区, 愿景 打破闭塞，拉进你我，分享知识，共同进步，努力创造更加友善进取的技术圈。

## 致谢
我也是一个平凡人, 编程这东西怎么说呢 , 自我理解的话, 虽然我学了这么多 但是总觉得自己有好多东西要学(其实本来就是, 时刻学习, 终身学习)
当时高考上来的, 刚来的时候对编程一脸懵逼, 但是遇到了好多帮助我的学长学姐以及同届的大佬相助, 在这里对每一个曾经帮助我的学长学姐以及同届大佬们道一声 "谢谢你们",
我的编程也没什么天赋, 但是心里知道自己的大体方向, 接下来就是埋头自学(笨鸟先飞的道理还是懂得), 对编程的热情不减, 无论35岁以后如何, 我希望自己永远不要忘记此刻对编程的热爱.


看完英雄本色最喜欢的一句话。 



>我等了三年，就是要等一个机会，我要争一口气，不是证明我了不起，我是要告诉大家，我失去的东西我一定要亲手拿回来」 --《英雄本色》

- 人生分为不同阶段, 你上一个阶段很失败, 不要丢失下一阶段的信心
- There is only one heroism in the world: to see the world as it is and to love it. 
- 事可为全力而为.

2020.9.12   Xinze Ma  花名   邱节

<center><font color=BBBBBB size=5>本站微信公众号</font></center>

![mark](https://s1.ax1x.com/2020/07/17/UsFeJJ.jpg)

<script>
function secondToDate(second) {
     if (!second) {
         return 0;
     }
     var time = new Array(0, 0, 0, 0, 0);
     if (second >= 365 * 24 * 3600) {
        time[0] = parseInt(second / (365 * 24 * 3600));
        second %= 365 * 24 * 3600;
    }
    if (second >= 24 * 3600) {
        time[1] = parseInt(second / (24 * 3600));
        second %= 24 * 3600;
    }
    if (second >= 3600) {
        time[2] = parseInt(second / 3600);
        second %= 3600;
    }
    if (second >= 60) {
        time[3] = parseInt(second / 60);
        second %= 60;
    }
    if (second > 0) {
        time[4] = second;
    }
    return time;
};
function setTime() {
         // 博客创建时间秒数，时间格式中，月比较特殊，是从0开始的，所以想要显示5月，得写4才行，如下
         var create_time = Math.round(new Date(Date.UTC(2019, 8, 11, 18, 37, 16)).getTime() / 1000);// 当前时间秒数,增加时区的差异
         var timestamp = Math.round((new Date().getTime() + 8 * 60 * 60 * 1000) / 1000);
         currentTime = secondToDate((timestamp - create_time));
         if (currentTime[0]==0){
             currentTimeHtml = currentTime[1] + '天'+ currentTime[2] + '时' + currentTime[3] + '分' + currentTime[4] + '秒';
         }else{
             currentTimeHtml = currentTime[0] + '年' + currentTime[1] + '天' + currentTime[2] + '时' + currentTime[3] + '分' + currentTime[4] + '秒';
         }
         // 兼容pjax，当htmer_time存在时输出，否则清空计时器
         if (document.getElementById("htmer_time")){
             document.getElementById("htmer_time").innerHTML = currentTimeHtml;
         }else{
              clearInterval(timer);
         }
}
var timer = setInterval(setTime, 1000);
</script>
