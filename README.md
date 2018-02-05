
# udn-newmedia-vue-components
聯合報新媒體中心 vue.js 組件

[![github version](https://img.shields.io/github/release/udn-newmedia/udn-newmedia-vue-components.svg)](https://github.com/udn-newmedia/udn-newmedia-vue-components/releases/) [![npm version](https://img.shields.io/npm/v/udn-newmedia-vue-components.svg)](https://www.npmjs.com/package/taiwan-vue-components) [![PRs welcome](https://img.shields.io/badge/PRs-welcome-ff69b4.svg)](https://github.com/udn-newmedia/udn-newmedia-vue-components/pulls) [![code with hearth by Udn Newmedia Eng.](https://img.shields.io/badge/Udn%20Newmedia-Eng.-brightgreen.svg)](https://github.com/udn-newmedia)

## Install

```
$ npm install udn-newmedia-vue-components --save
```

## Usage

import 想用的 components，EX:

```js
<template>
	<App>
		<Indicator color="#FFFFFF" />
		<Quote text="引言" />
	</App>
</template>

import {Indicator, Content, Quote} from 'udn-newmedia-vue-components'

new Vue({
	components: {
    	Indicator, Content, Quote
    }
})
```

### Demo Page

[Demo LongForm](https://udn-newmedia.github.io/udn-newmedia-vue-components/)

[Demo Page](https://udn-newmedia.github.io/udn-newmedia-vue-components/page.html)


### Components

+ Indicator

	頁面上方進度條
```js
<Indicator color="#FF0000"></Indicator>
```
	###### - Props

	* [color] 進度條顏色 預設: #AA4444

+ Head-Bar
```js
<Head-Bar Menu-Slide-From="top" Bg-Color="transparent"></Head-Bar>
```
    ##### - Props

	* [BgColor] 頁頭背景色 預設: #000
  	* [MenuSlideFrom] 選單滑入點 預設: top , value: top, left, right, bottom

+ Cover

	封面
```js
<Cover title="好好說再見" subtitle="插畫記林杰樑走後1500天" bg="./static/bg_wang.jpg" bgweb="./static/web/bg_wang.jpg" position="middle"></Cover>
```
	##### Props

	* [title] 大標
	* [subtitle] 副標
	* [bg] 手機板封面圖
	* [bgweb] 網頁版封面圖
	* [position] 標題位置 有 top middle bottom center 4種

+ Content-Container

	用於包內文，內含內文行高等CSS設定
```js
<Content-Container background-color="#FFFFFF">
	<p>再過43年，台灣幾乎人人都可以活到90歲，但活得長，卻不一定能活得好。高齡化下一階段最大挑戰，將變成「活著要幹嘛」？</p>
	<p><br/></p>
	<p>面對變長的人生下半場，有些人不退也不休，利用上半場累積的經驗與智慧，開創第二春傳承給下一代。有人則急流勇退，人生下半場追求自我實現。</p>	
</Content-Container>
```  
    ##### - Props
    
    * [background-color] 區塊背景色 預設: 無

+ Column-One

	1格圖片排列
```js
<Column-One imgsay="圖說" img1="./static/bg_wang.jpg" imgweb1="./static/web/bg_wang.jpg"></Column-One>
```
	##### - Props

	* [img1] 圖片1
	* [imgsay] 圖說

+ Column-Two

	2格圖片排列
```js
<Column-Two imgsay="圖說" img1="./static/bg_wang.jpg" img2="./static/bg_wang.jpg" imgweb1="./static/web/bg_wang.jpg" imgweb2="./static/web/bg_wang.jpg"></Column-Two>
```
	##### - Props

	* [img1~2] 圖片1~2
	* [imgsay] 圖說

+ Column-Three

	3格圖片排列
```js
<Column-Three imgsay="圖說" img1="./static/bg_wang.jpg" img2="./static/bg_wang.jpg" img3="./static/bg_wang.jpg" imgweb1="./static/web/bg_wang.jpg" imgweb2="./static/web/bg_wang.jpg" imgweb3="./static/web/bg_wang.jpg"></Column-Three>
```
	##### - Props

	* [img1~3] 圖片1~3
	* [imgsay] 圖說

+ Quote

	內文引言區塊，內含引言CSS設定
```js
<Quote img="./static/lee.png" text="＂未來老人不會忙著生病，會愈來愈健康＂＂未來老人不會忙著生病，會愈來愈健康＂＂未來老人不會忙著生病，會愈來愈健康＂＂未來老人不會忙著生病，會愈來愈健康＂＂未來老人不會忙著生病，會愈來愈健康＂" refer="-- 陳亮恭"/>
``` 
    ##### - Props

	* [img] 人頭圖
	* [text] 引言內文
  	* [refer] 引言者
  	* [color] 引言文字顏色 預設:#888888
  	* [border-color] 引言框顏色

+ Youtube

	youtube嵌入
```js
<Youtube src="https://www.youtube.com/embed/kMguxxwW_-A"></Youtube>
```
	##### - Props

	* [src] 連結網址

+ Section-Fixed-Bg

	滾動視差過場
```js
<Section-Fixed-Bg text="王琄認為，大齡這個階段，是人生中最好、最穩定的狀態。" bg="./static/bg_wang.jpg" bgweb="./static/web/bg_wang.jpg" position="center"></Section-Fixed-Bg>
```
	##### - Props

	* [text] 過場文字
	* [bg] 手機圖
	* [bgweb] 網頁圖
	* [position] 文字位置 有 center 跟 bottom 兩種

+ Section-Bg

	滿版圖過場
```js
<Section-Bg bg="./static/bg_wang.jpg" bgweb="./static/web/bg_wang.jpg" imgsay="陳智遠（左圖）將老港味轉為深度旅遊的商機，頗受遊客歡迎。"></Section-Bg>
```
	##### - Props

	* [bg] 手機圖
	* [bgweb] 網頁圖
	* [imgsay] 圖說

+ Question

	問卷問題

	##### - Props

	* [href] 表單連結位置
	* [text] 文字

+ Editor
	
    作者區塊，內含CSS設定
```js
<Editor>
     <div>文字：蔡佩蓉、洪欣慈</div>
     <div>視覺設計、影音：張心慈、許瑋琳</div>
     <div>網頁製作：鄭偉廷</div>
     <div>攝影：許正宏</div>
     <div>場地提供：一直是晴天</div>
     <div>2017.10.30</div>
</Editor>
```   

    ##### - Props
    
    * None

+ Logo

	頁面 Logo 區塊
    
    ##### - Props
    
    * None

+ Relate

	延伸閱讀區塊，內含CSS設定
```js
<Relate title="延伸閱讀" color="#363434" 
	href1="https://p.udn.com.tw/upf/newmedia/2016_data/20161003_quicksand_middle_age/index.html" img1="./static/web/bg_wang.jpg" text1="我們長大，把光亮帶回黑暗家鄉" 
	href2="https://p.udn.com.tw/upf/newmedia/2016_data/20161003_quicksand_middle_age/index.html" img2="./static/web/bg_wang.jpg" text2="助脫貧…教技能 推存錢帳戶" 
	href3="https://p.udn.com.tw/upf/newmedia/2016_data/20161003_quicksand_middle_age/index.html" img3="./static/web/bg_wang.jpg" text3="兒少發展帳戶推動3個月 申請率25%" 
	href4="https://p.udn.com.tw/upf/newmedia/2016_data/20161003_quicksand_middle_age/index.html" img4="./static/web/bg_wang.jpg" text4="流沙中年 棄6萬月新顧爸媽，我在貧窮線下度日" > 
</Relate>
```
    ##### - Props
    
    * [title] 延伸閱讀
	* [color] 文字顏色
	* [href1~4] 連結 1~4
	* [img1~4] 圖片 1~4
	* [text1~4] 文字 1~4

+ Share

	FB and Line 分享區塊。
```js
<Share href="https://udn.com/upf/newmedia/2017_data/ideal/index.html"></Share>
```
    ##### - Props
    
    * [href] 分享用網址 (必填)

+ Fb-Comment

	FB 留言 plugin。
```js
<Fb-Comment href="https://udn.com/upf/newmedia/2017_data/ideal/index.html"></Fb-Comment>
```
    ##### - Props
    
    * [href] 分享用網址 (必填)

+ Foot

	頁腳
```js
<Foot background-color="#FFFFFF"></Foot>
```
	##### - Props

	* [background-color] 區塊背景色 預設: 無

+ Bodymovin
	
	使用 Bodymovin 套件，產生網頁動畫。(需要import lottie-web)

	##### - Props

	* [jsonfile] 輸入`.json`檔

+ EmbededVideo

	嵌入文章中之影片

	##### - Props

	* [src] 影片位址 (mobile版)

	* [src-web] 影片位址 (pc版)

	* [poster] 影片預覽圖 (mobile版)

	* [poster-web] 影片預覽圖 (pc版)

	* [background-color] 背景色
	
	* [custom-control] 是否使用自定義樣式
+ ImageContain

	嵌入文章中的圖片

	##### - Props

	* [width] 圖片寬 (mobile版)

	* [height] 圖片高 (mobile版)

	* [widthWeb] 圖片寬 (pc版)

	* [heightWeb] 圖片高 (pc版)

	* [src] 圖片位址 (mobile版)

	* [srcWeb] 圖片位址 (pc版)

+ PhotoComparison

	兩張照片互相比對 (ex. 新舊照片對照)

	##### - Props

	* [text] 出現在最下方的說明文字

	* [src-old] 舊照片位址 (mobile版)

	* [src-new] 新照片位址 (mobile版)

	* [src-web-new] 新照片位址 (pc版)

	* [src-web-old] 舊照片位址 (pc版)

	* [src-mob-width] 照片寬 (mobile版)

	* [src-mob-height] 照片高 (mobile版)

	* [src-web-width] 照片寬 (pc版)

	* [src-web-height] 照片高 (pc版)

	* [data-target] 可賦予編號

+ Page

	滿版滾動容器，所有的版面都要放在裡面。

```js
<Page>
    <Page-Cover title="好好說再見" subtitle="插畫記林杰樑走後1500天" bg="./static/bg_wang.jpg" bgWeb="./static/web/bg_wang.jpg" position="bottom" fontcolor="#fff"></Page-Cover>
    <Page-Intro fontcolor="#fff" Bg-Color="#000"></Page-Intro>
    <Page-Card Video-Src='static/video.mp4'></Page-Card>
</Page>
```

   #####Props

	* [scroll-speed] 滿版滾動速度, 預設700 ex: scroll-speed=1000	 	 

+ page-head-bar

	page的head-bar。 請放在page標籤外!。
	該標籤會自動抓 page-cover 中的 title內容。
	如需外連區塊則在`<page-head-bar>`內 置入 `<a>`。

```js
<page-head-bar href='https://udn.com/upf/newmedia/2017_data/universide_taipei_2017/jump_boys.html' youtube='yes'>
    <a href='./page.html'>外連結1</a>
    <a href='./page.html'>外連結2</a>
    <a href='./page.html'>外連結3</a>
</page-head-bar>
```


   ##### Props
	* [href] Facebook Comment href參數(必填)
	* [color] icon和導引字顏色 預設:白字 手機只變icon顏色
	* [bg-color] headrbar的顏色
	* [youtube] youtube Icon 
	* [youtube-link] youtube 連結

+ page-cover

	滿版標題Cover

```js
<Page-Cover title="李志凱" subtitle="15秒翻滾人生 拚一秒完美落地" bg="./static/m-bg_s.jpg" bgWeb="./static/m-bg.jpg" position="bottom" fontcolor="#fff" 
arrow-color='#fff' hint='yes' hint-color='#fff'></Page-Cover>
```
    ##### Props

	* [title] 大標
	* [subtitle] 副標
	* [font-color] 大/副題顏色
	* [bg] 手機封面圖
	* [bg-web] 網頁封面圖
	* [position] 標題位置 有 top middle bottom 3種	
	* [arrow-color] 向下提示箭頭顏色
	* [hint] 是否需要向下滾動提示字樣
	* [hint-color] 提示字樣顏色

+ PageIntro

	滿版引言

```js
<Page-Intro font-color="#fff" bg="./static/w1-bg_s.jpg" bg-web="./static/w1-bg2.jpg" arrow-color='#fff' hint-color='#fff'>
   <p>「不拚什麼都沒有！」21歲競技體操國手李智凱，曾經是紀錄片《翻滾吧！男孩》中的「菜市場凱」，從小苦練「湯瑪士迴旋」絕技，讓他在去年為台灣搶下睽違16年的奧運體操門票，也讓世界注意到台灣體操選手。</p>
   <p><br/></p>
   <p>這次在台北世大運鞍馬決賽，李智凱以完美表現，摘下我國在世大運史上首面鞍馬金牌（奪金時刻影片）。他說：「努力過、嘗試過至少有50%的機會，不嘗試的話等於0。」不怕失敗，愈戰愈勇，就是他能在體操路上堅持15年的原因。</p>
   <h6>2017.08.25更新</h6>
   <Share href="http://10.116.80.31:3000/udn-newmedia-vue-components/page.html"/>
</Page-Intro>
```	
+ PageCard

   page卡片，可放入圖片，影片，或純文字

   影片範例

```js
<Page-Card video-src='./static/video/pcvideo.mp4' video-src-web='static/video/pcvideo.mp4' video-poster="./static/bg_wang.jpg" video-poster-web='static/bg_wang.jpg' bg-color='#000'>
    <p>專注地盯著眼前的鞍馬，深吸一大口氣，為自己注入信心，緊握把手、一躍而上，雙腿在空中如疾風般旋轉。</p>
    <p><br/></p>
    <p>世大運前十天，李智凱在競技體操測試賽中，展現獨家招式「湯瑪士迴旋」，華麗美技讓外國選手讚嘆。</p>
</Page-Card> 
```

   圖片範例

```js
<Page-Card Img-Src='./static/imageSmaple.png'>
    <p>專注地盯著眼前的鞍馬，深吸一大口氣，為自己注入信心，緊握把手、一躍而上，雙腿在空中如疾風般旋轉。</p>
    <p><br/></p>
    <p>世大運前十天，李智凱在競技體操測試賽中，展現獨家招式「湯瑪士迴旋」，華麗美技讓外國選手讚嘆。</p>
</Page-Card>  	
```	

   純文字範例

```js
<Page-Card>
    <p>專注地盯著眼前的鞍馬，深吸一大口氣，為自己注入信心，緊握把手、一躍而上，雙腿在空中如疾風般旋轉。</p>
    <p><br/></p>
    <p>世大運前十天，李智凱在競技體操測試賽中，展現獨家招式「湯瑪士迴旋」，華麗美技讓外國選手讚嘆。</p>
    <p><br/></p>
    <p>世大運前十天，李智凱在競技體操測試賽中，展現獨家招式「湯瑪士迴旋」，華麗美技讓外國選手讚嘆。</p>
</Page-Card>	
```	

   純文字 + 引文 +標題範例

```js
<page-card title='小學門口 大海送垃圾' font-color='#000' bg='./static/bg_mobile.jpg' bg-web="./static/bg.jpg" box-color='#fff' use-quote='yes'>
 <p>專注地盯著眼前的鞍馬，深吸一大口氣，為自己注入信心，緊握把手、一躍而上，雙腿在空中如疾風般旋轉。</p>
 <p><br/></p>
 <p>世大運前十天，李智凱在競技體操測試賽中，展現獨家招式「湯瑪士迴旋」，華麗美技讓外國選手讚嘆。</p>
 <p><br/></p>
 <p>世大運前十天，李智凱在競技體操測試賽中，展現獨家招式「湯瑪士迴旋」，華麗美技讓外國選手讚嘆。</p>                
</page-card>  
```

    ##### Props

	* [title] 卡片標題
    * [video-src] 影片來源
    * [video-poster] 影片預覽圖
    * [video-src-web] 電腦版影片來源
    * [video-poster-web] 電腦版預覽圖來源
    * [img-src] 圖片來源
    * [img-say] 圖片說(alt, title)
    * [bg-color] 背景色
    * [font-color] 字體顏色
    * [box-color] 卡片背景色
    * [bg] 手機背景圖
    * [bg-web] 網頁背景圖
    * [use-quote] 使用引言 ex: use-quote='yes'
    * [quote-first] 引言在前面 ex: quote-first='yes'
    
+ PageFullvideo

  page滿版影音

```js
<Page-Fullvideo src='./static/video/mobvideo.mp4' src-web='./static/video/pcvideo.mp4'></Page-Fullvideo>  
```	

	##### Props

	* [src] 手機影片來源
	* [poster] 手機愈覽圖
	* [src-web] 電腦版影片來源
	* [poster-web] 電腦版預覽圖
	* [bg-color] 背景色

+ PageQuote
  
  page引言

```js
<Page-Quote quoter="體操國手 李智凱" src='static/squareVideo.mp4' src-web='./static/squareVideo.mp4' bg-color='#82c539'>
    <p>奧運失敗的時候，當下腦筋是一片空白的，什麼都沒有想法，就是最不想發生的事發生了。下一個想法就是我還在比賽，要把比賽完成。</p>
</Page-Quote>  
``` 

	##### Props

	* [bg-color] 版面背景色
	* [box-color] 內文區塊背景色
	* [qouter] 引言來源
	* [src] 影片來源
	* [src-web] 電腦版影片來源
	* [poster] 預覽圖來源
	* [poster-web] 電腦版預覽圖來源

+ PageImgsay

  滿版圖說

  圖說文字用 `p` 輸入

```js
<Page-Imgsay src="./static/bg_wang.jpg" src-web="static/web/bg_wang.jpg">
    <p>學童突發奇想，將廢棄漁業浮球做成樂器吹奏。</p>
</Page-Imgsay>
```

	#####Props

	* [src] 圖片來源
	* [src-web] 電腦版圖片來源

+ PageFooter

  Page最後一頁

  製作群請用 `p` 輸入

```js
<page-footer 
    href="http://10.116.80.31:3000/udn-newmedia-vue-components/page.html"
    bg-img='./static/bg_mobile.jpg' bg-img-web='./static/bg.jpg'
    color="#fff" bg-color='#000' udncom='yes' newmedia='yes' update='2017.05.25更新'
    link1='https://goo.gl/wJMfCh' text1='競技體操的秘密 選手如何對抗地心引力' img1='https://udn.com/upf/newmedia/image/projects/201706_hk20.jpg'
    link2='https://goo.gl/iVf5H8' text2='為同一個名字努力' img2='https://udn.com/upf/newmedia/image/projects/201706_hk20.jpg'
    link3='https://goo.gl/wJMfCh' text3='跆拳道得分5招 國首示範給你看' img3='https://udn.com/upf/newmedia/image/projects/201706_hk20.jpg'
    link4='https://goo.gl/iVf5H8' text4='我只是範例' img4='https://udn.com/upf/newmedia/image/projects/201706_hk20.jpg'>
    <p>製作團隊：</p>
    <p>文字：魏妤庭、連珮宇</p>
    <p>攝影：許正宏、王騰毅</p>
    <p>網頁製作：方泰鈞</p>
    <p>監製：林新輝、鄭朝陽、董谷音、蔡幸怡</p>
</page-footer>
```

	#####Props

	*[href] 分享出去的連結網址
	*[bg-img] 手機版背景圖
	*[bg-img-web] 電腦版背景圖
	*[color] 字體顏色
	*[bg-color] 滿版背景色
	*[udncom] 使用聯合新聞網Logo ex: udncom='yes'
	*[newmedia] 使用新媒體中心Logo ex: newmedia='yes'
	*[ubrand] 使用融媒體Logo ex: ubrand='yes'
	*[link1~4] 延伸閱讀1~4連結
	*[text1~4] 延伸閱讀1~4標題
	*[img1~4] 延伸閱讀1~4圖