---
layout: post
title:  "Gradle构建SSM环境一"
date:   2016-09-06
image: fruits.jpg
description: 使用Gradle构建整合Spring,SpringMvc,Mybatis
tags: [Gradle, Spring, SpringSecurity, Mybatis, Intellij, SpringMVC, Java, Jsp, JavaWeb]

---

#### 前言
#### 准备
#### 创建Gradle项目
#### 引入项目依赖类库（SSM类库）
#### 配置SpringMVC环境（xml）
#### 配置Mybatis环境（xml）
#### 编写HelloWorld

<style>
.marquee {
  width: 100%;
  padding: 0.5em 0;
  margin: 0 auto;
  overflow: hidden;
  background-color: #f6f6f6;
  margin-bottom: 30px;
  position: relative;
  text-align: left;
}

.marquee p:after {
  content: "";
  white-space: nowrap;
  padding-right: 50px;
}

.marquee p {
  margin: 0;
  padding-left: 100%;
  display: inline-block;
  white-space: nowrap;
  -webkit-animation-name: marquee;
  -webkit-animation-timing-function: linear;
  -webkit-animation-duration: 10s;
  -webkit-animation-iteration-count: infinite;
  -moz-animation-name: marquee;
  -moz-animation-timing-function: linear;
  -moz-animation-duration: 10s;
  -moz-animation-iteration-count: infinite;
  -ms-animation-name: marquee;
  -ms-animation-timing-function: linear;
  -ms-animation-duration: 10s;
  -ms-animation-iteration-count: infinite;
  -o-animation-name: marquee;
  -o-animation-timing-function: linear;
  -o-animation-duration: 10s;
  -o-animation-iteration-count: infinite;
  animation-name: marquee;
  animation-timing-function: linear;
  animation-duration: 10s;
  animation-iteration-count: infinite;
  text-align: left;
}

@-webkit-keyframes marquee {
  from {
    -webkit-transform: translate(0);
  }

  to {
    -webkit-transform: translate(-150%);
  }
}

@-moz-keyframes marquee {
  from {
    -moz-transform: translate(0);
  }

  to {
    -moz-transform: translate(-150%);
  }
}

@-ms-keyframes marquee {
  from {
    -ms-transform: translate(0);
  }

  to {  
    -ms-transform: translate(-150%);
  }
}

@-o-keyframes marquee {
  from {
    -o-transform: translate(0);
  }

  to {
    -o-transform: translate(-150%);
  }
}

@keyframes marquee {
  from {
    transform: translate(0);
  }

  to {
    transform: translate(-150%);
  }
}
</style>
<div class="marquee">
<p>欢迎来到App Hack.</p>
</div>


#### html写法
{% highlight html %}
<div class="marquee">
<p>欢迎来到App Hack.</p>
</div>
{% endhighlight %}


#### css写法
{% highlight css %}
.marquee {
  width:600px;
  padding:0.5em 0;
  overflow:hidden;
  background-color:#f6f6f6;
  margin-bottom:10px;
  position:relative;
}

.marquee p:after {
  content:"";
  white-space:nowrap;
  padding-right:50px;
}

.marquee p {
  margin:0;
  padding-left:600px;
  display:inline-block;
  white-space:nowrap;
  -webkit-animation-name:marquee;
  -webkit-animation-timing-function:linear;
  -webkit-animation-duration:10s;
  -webkit-animation-iteration-count:infinite;
  -moz-animation-name:marquee;
  -moz-animation-timing-function:linear;
  -moz-animation-duration:10s;
  -moz-animation-iteration-count:infinite;
  -ms-animation-name:marquee;
  -ms-animation-timing-function:linear;
  -ms-animation-duration:10s;
  -ms-animation-iteration-count:infinite;
  -o-animation-name:marquee;
  -o-animation-timing-function:linear;
  -o-animation-duration:10s;
  -o-animation-iteration-count:infinite;
  animation-name:marquee;
  animation-timing-function:linear;
  animation-duration:10s;
  animation-iteration-count:infinite;
}
@-webkit-keyframes marquee {
  from   { -webkit-transform: translate(0%);}
  99%,to { -webkit-transform: translate(-100%);}
}
@-moz-keyframes marquee {
  from   { -moz-transform: translate(0%);}
  99%,to { -moz-transform: translate(-100%);}
}
@-ms-keyframes marquee {
  from   { -ms-transform: translate(0%);}
  99%,to { -ms-transform: translate(-100%);}
}
@-o-keyframes marquee {
  from   { -o-transform: translate(0%);}
  99%,to { -o-transform: translate(-100%);}
}
@keyframes marquee {
  from   { transform: translate(0%);}
  99%,to { transform: translate(-100%);}
}
{% endhighlight %}





