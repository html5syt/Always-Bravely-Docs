<div style="text-align:center;"> <h1><b>全站使用说明（未迁移完成）</b></h1></div>

---
## 欢迎各位成员！


<div style="text-align:center;"> <h1 style="color: red"><b>请认真阅读完以下重点内容！</b></h1></div>

1. **注册规则在2.1节！**
2. **此社区不对所有成年人开放，请勿在校内大幅度宣传！（懂得都懂）**
3. **本文部分图片由于功能变动与社区实际情况有出入，请以实际社区操作为准！**

---
---
title: Home
hide:
  # - navigation # 显示右
  # - toc #显示左
  - footer
  - feedback
comments: false
---
# 主页

<center><font  color= #02A6F2 size=6 class="ml3">“欢迎循此苦旅，以达星辰”</font></center>
<script src="https://cdnjs.cloudflare.com/ajax/libs/animejs/2.0.2/anime.min.js"></script>



<!-- ！时间 -->
<div id="rcorners2" >
  <div id="rcorners1">
    <!-- <i class="fa fa-calendar" style="font-size:100"></i> -->
    <body>
      <font color="#4351AF">
        <p class="p1"></p>
<script defer>
    //格式：2020年04月12日 10:20:00 星期二
    function format(newDate) {
        var day = newDate.getDay();
        var y = newDate.getFullYear();
        var m =
            newDate.getMonth() + 1 < 10
                ? "0" + (newDate.getMonth() + 1)
                : newDate.getMonth() + 1;
        var d =
            newDate.getDate() < 10 ? "0" + newDate.getDate() : newDate.getDate();
        var h =
            newDate.getHours() < 10 ? "0" + newDate.getHours() : newDate.getHours();
        var min =
            newDate.getMinutes() < 10
                ? "0" + newDate.getMinutes()
                : newDate.getMinutes();
        var s =
            newDate.getSeconds() < 10
                ? "0" + newDate.getSeconds()
                : newDate.getSeconds();
        var dict = {
            1: "一",
            2: "二",
            3: "三",
            4: "四",
            5: "五",
            6: "六",
            0: "天",
        };
        //var week=["日","一","二","三","四","五","六"]
        return (
            y +
            "年" +
            m +
            "月" +
            d +
            "日" +
            " " +
            h +
            ":" +
            min +
            ":" +
            s +
            " 星期" +
            dict[day]
        );
    }
    var timerId = setInterval(function () {
        var newDate = new Date();
        var p1 = document.querySelector(".p1");
        if (p1) {
            p1.textContent = format(newDate);
        }
    }, 1000);
</script>
      </font>
    </body>
  </div>
  开发中，站点变动较大，请谅解！
</div> 




<body>
    <font color="#B9B9B9">
    <p style="text-align: center; ">
            <span>（未启用）本站已经运行</span>
            <span id='box1'></span>
</p>
  <div id="box1"></div>
  <script>
    function timingTime(){
      let start = '2022-10-20 00:00:00'
      let startTime = new Date(start).getTime()
      let currentTime = new Date().getTime()
      let difference = currentTime - startTime
      let m =  Math.floor(difference / (1000))
      let mm = m % 60  // 秒
      let f = Math.floor(m / 60)
      let ff = f % 60 // 分钟
      let s = Math.floor(f/ 60) // 小时
      let ss = s % 24
      let day = Math.floor(s  / 24 ) // 天数
      return day + "天" + ss + "时" + ff + "分" + mm +'秒'
    }
    setInterval(()=>{
      document.getElementById('box1').innerHTML = timingTime()
    },1000)
  </script>
  </font>
</body>

