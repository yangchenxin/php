<title>河北中学</title> <script type="text/javascript" src="{JS_PATH}/HBschool/jquery-1.8.2.min.js"></script> <script type="text/javascript" src="{JS_PATH}/HBschool/solideForK13-min.js"></script> <script type="text/javascript" src="{JS_PATH}/HBschool/ad_pic.js"></script>
网站首页
{pc:content action="category" catid="0" order="listorder ASC" num="11" siteid="$siteid"}
               <!-- 显示出来$v代表11条数据 -->

               	{loop $data $v}
               		<!--这里面是找一对li写出结构-->
               		<li><a href="{$v['url']}">{$v['catname']}</a></li>
               		<!--在数据库中category中找到栏目名称对应的内容-->
               			

               	{/loop}{/pc}
                <!-- <li>网站首页</li>
                <li><a href="list.html">学校概况</a></li>
                <li><a href="#">规章制度</a></li>
                <li><a href="#">德育网</a></li>
                <li><a href="#">教研网</a></li>
                <li><a href="#">名师风采</a></li>
                <li><a href="#">高考专栏</a></li>
                <li><a href="#">图书馆</a></li>
                <li><a href="#">校友会</a></li>
                <li><a href="#">河中论坛</a></li>
                <li><a href="#">查询系统</a></li>
                <li><a href="#" class="specil">东校区</a></li>  -->                   
            </ul>
        </div>
        <div id="search">
        <input name="search" type="text" class="search_text" /><input name="searchbut" type="button" class="search_but" value=" " />
        </div>
    </div>
    <div id="no1">
    	<div id="picnews">
        
       	 <div class="container" id="idTransformView">

adfasdfsadf

adfasdfsadf

{pc:content action="lists" catid="21" order="inputtime DESC" num="8"} {loop $data $v}
{$v['title']} {date('Y-m-d',$v['inputtime'])}
{/loop}{/pc}
             </div>
        </div>
      <div id="notice">
      	<h1><a href="#"><img src="{IMG_PATH}/HBschool/30.gif" width="30" height="9" /></a></h1>
        <ul>
        <!--校园公告-->
          {pc:content 
                <!-- 获取出来 -->
               action="lists"
               catid="22" 
               order="inputtime DESC"
               num="4"}
               <!-- 显示出来$v代表八条数据 -->
               	{loop $data $v}
               			<li><a href="{$v['url']}"><img src="{IMG_PATH}/HBschool/pot.gif" width="4" height="4" /> {$v['title']} {date('Y-m-d',$v['inputtime'])}</a></li>
               			
               	{/loop}{/pc}
       	  <!-- <li><a href="#" ><img src="{IMG_PATH}/HBschool/pot.gif" width="4" height="4" /> 河北中学男子篮球体育特长生招生简章 (2013-04-11)</a></li>
               	<li><a href="#" ><img src="{IMG_PATH}/HBschool/pot.gif" width="4" height="4" /> 河北中学音乐特长生复试名单 (2013-04-08)</a></li>
                <li><a href="#"><img src="{IMG_PATH}/HBschool/pot.gif" width="4" height="4" /> 河北中学2013年艺术特长生招生简章 (2013-03-01)</a></li>
                <li><a href="#"><img src="{IMG_PATH}/HBschool/pot.gif" width="4" height="4" /> 2012-2013第二学期考试、放假安排 (2013-02-25) </a></li> -->
        </ul>
      </div>
    </div>
  <div id="no2">
    	<div class="news_content">
        	<h1><img src="{IMG_PATH}/HBschool/news_jy_title.gif" width="480" height="40" usemap="#Map" border="0" alt="教研网" />
              <map name="Map" id="Map">
                <area shape="rect" coords="439,11,481,33" href="{APP_PATH}index.php?m=content&c=index&a=lists&catid=13"" />
              </map>
        	</h1>
     		<img src="{IMG_PATH}/HBschool/news_jy_pic.gif" width="130" height="165" alt="tp" />
             <ul>
             <!--河中教研网-->
             	 {pc:content 
                <!-- 获取出来 -->
               action="lists"
               catid="13" 
               order="inputtime DESC"
               num="6"}

               <!-- 显示出来$v代表6条数据 -->

               	{loop $data $v}
               			<li><a href="{$v['url']}">{$v['title']}</a> </li> 
               			
               			

               	{/loop}{/pc}

            	<!-- <li><a href="#">[公开课教学][图文]化学老师于文英举办观摩课活动</a> </li> 
				<li><a href="#">[公开课教学][图文]本部数学组组织公开课教学校调研 </a> </li> 
				<li><a href="#">[公开课教学][图文]生物老师开展观摩课活动</a> </li>  
				<li><a href="#">[教学交流][组图]文科部高一年级召开期中考试分析…</a> </li>  
				<li><a href="#">[教与学][图文]【教与学】打破思维定势走出误区…</a> </li>  
				<li><a href="#">[教学交流][组图]石家庄市教科所专家来我</a> </li>  -->
            </ul>
      </div>
        <div class="news_content" style="margin-left:45px; _margin-left:25px">
        	<h1><img src="{IMG_PATH}/HBschool/news_dy_title.gif" width="480" height="40" usemap="#Map" border="0" alt="教研网" />
              <map name="Map" id="Map">
                <area shape="rect" coords="439,11,481,33" href="{APP_PATH}index.php?m=content&c=index&a=lists&catid=12"" />
              </map>
        	</h1>
     		<img src="{IMG_PATH}/HBschool/news_dy_pic.gif" width="130" height="165" alt="tp" />
            <ul>
            <!--这个是德育网-->
            	 {pc:content 
                <!-- 获取出来 -->
               action="lists"
               catid="13" 
               order="inputtime DESC"
               num="6"}
               <!-- 显示出来$v代表6条数据 -->
               	{loop $data $v}
               			<li><a href="{$v['url']}">{$v['title']}</a> </li> 
               			
               			
               	{/loop}{/pc}
            	<!-- <li><a href="#">[公开课教学][图文]化学老师于文英举办观摩课活动</a> </li> 
				<li><a href="#">[公开课教学][图文]本部数学组组织公开课教学校调研 </a> </li> 
				<li><a href="#">[公开课教学][图文]生物老师开展观摩课活动</a> </li>  
				<li><a href="#">[教学交流][组图]文科部高一年级召开期中考试分析…</a> </li>  
				<li><a href="#">[教与学][图文]【教与学】打破思维定势走出误区…</a> </li>  
				<li><a href="#">[教学交流][组图]石家庄市教科所专家来我</a> </li>  -->
            </ul>
        </div>
      </div>
  <div id="no4">
  	<div id="synopsis">
     <img src="{IMG_PATH}/HBschool/gnq.gif" width="258" height="260" usemap="#Map4" style="margin-top:10px;" border="0"/>
     <map name="Map4" id="Map4">
       <area shape="rect" coords="144,133,250,240" href="成绩查询" />
       <area shape="rect" coords="12,129,119,239" href="通讯录" />
       <area shape="rect" coords="9,6,116,113" href="视频" />
       <area shape="rect" coords="140,9,243,114" href="班级空间" />
     </map>
    </div>
    <div id="slide_1">
	<div class="slide_content">
		<ul>
			{pc:content action="lists" catid="24" num="6" order="inputtime DESC"}
{loop $data $v}
<li>          
<a href="{$v['url']}"><img src="{$v['thumb']}" alt="{$v['title']}" width="200px" height="150px"></a>
<p>{$v['title']}</p>
{/loop} {/pc}
友情链接

邯郸市第一中学的网站
邯郸市第一中学
邯郸市第一中学
邯郸市第一中学
邯郸市第一中学
友情链接

邯郸市第一中学的网站
邯郸市第一中学
邯郸市第一中学
邯郸市第一中学
邯郸市第一中学
      </div>
      
      <div class="foot_link">
    	<h1><img src="{IMG_PATH}/HBschool/foot_down.gif" width="150" height="36" alt="资源下载" /></h1>
        <ul>
        	<li><a href="#">[资源中心]教师班主任成绩公示系统</a></li>
            <li><a href="#">[资源中心]高考资源网</a></li>
            <li><a href="#">[资源中心]中学学科网系统</a></li>
            <li><a href="#">[资源中心]全品高考网</a></li>
            <li><a href="#">[资源中心]志鸿网园校办公系统</a></li>
        </ul>            
      </div>
      
          <div class="foot_link" style="margin-right:0">
    	<h1><img src="{IMG_PATH}/HBschool/foot_count.gif" width="150" height="36" alt="网站统计" /></h1>
        <ul>
        	<li>总访问量：2600700</li>
            <li>人总浏览量：3482048人</li>
            <li>今日访问：2506人</li>
            <li>日均访问：1653人</li>
            <li>当前在线：21人</li>
        </ul>            
      </div>
Copyright © 2008－2013 http://www.***.com All Rights Reserved 网站备案：冀ICP备00000000号


<script type="text/javascript"> $("#close").click(function(){ $(this).parent().css("display",'none'); }); </script>





#list

!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">

<title>河北中学</title>
网站首页
{pc:content action="category" catid="0" order="listorder ASC" num="11" siteid="$siteid"}
               <!-- 显示出来$v代表11条数据 -->

                {loop $data $v}
                    <!--这里面是找一对li写出结构-->
                    <li><a href="{$v['url']}">{$v['catname']}</a></li>
                    <!--在数据库中category中找到栏目名称对应的内容-->
                        

                {/loop}{/pc}
            	<!-- <li>网站首页</li>
                <li><a href="#">学校概况</a></li>
                <li><a href="#">规章制度</a></li>
                <li><a href="#">德育网</a></li>
                <li><a href="#">教研网</a></li>
                <li><a href="#">名师风采</a></li>
                <li><a href="#">高考专栏</a></li>
                <li><a href="#">图书馆</a></li>
                <li><a href="#">校友会</a></li>
                <li><a href="#">河中论坛</a></li>
                <li><a href="#">查询系统</a></li>
                <li><a href="#" class="specil">东校区</a></li>         -->            
            </ul>
        </div>           
    </div>
  <div id="dh">
        	<h1><a href="index.html">河北中学首页</a> - <a href="#">学校概况</a> - 所获荣誉</h1>
        	<div id="search">
        <input name="search" type="text" class="search_text" /><input name="searchbut" type="button" class="search_but" value=" " />
        </div>
      </div>
    <div id="left">
    	<div id="leftmenu">
        	<h1>学校概况</h1>
            <ul>
            	<a href="#">领导简介</a>
                <a href="#">学校简介</a>
                <a href="#">光荣历史</a>
                <a href="#" class="dq">所获荣誉</a>
                <a href="#">图说河中</a>
          </ul>
        </div>
      <div id="pic">
      <h1></h1>
       	<div id="colee" >
2010-2011年度先进单位

2010-2011年度先进单位

2010-2011年度先进单位

2010-2011年度先进单位

2010-2011年度先进单位

2010-2011年度先进单位

        </div>
    </div>
    
    <div id="right">
    	<h1><h1>{$catname}</h1></h1>
        <ul>
        {pc:content action="lists" catid="$catid" num="15" order="inputtime DESC" page="$page"}
{loop $data $v}

{str_cut($v['title'],90)} {date('Y-m-d',$v['inputtime'])}
{/loop} {/pc}
前一页123456后一页
  </div>

<div id="foot">	  
	Copyright © 2008－2013 http://www.***.com All Rights Reserved   网站备案：冀ICP备00000000号
</div>
<script type="text/javascript" src="js/pic.js"></script>




show1

<title>河北中学</title> <script type="text/javascript" src="{JS_PATH}/jquery.min.js"></script>
网站首页
{pc:content action="category" catid="0" order="listorder ASC" num="11" siteid="$siteid"}
               <!-- 显示出来$v代表11条数据 -->

                {loop $data $v}
                    <!--这里面是找一对li写出结构-->
                    <li><a href="{$v['url']}">{$v['catname']}</a></li>
                    <!--在数据库中category中找到栏目名称对应的内容-->
                        

                {/loop}{/pc}
            	<!-- <li>网站首页</li>
                <li><a href="list.html">学校概况</a></li>
                <li><a href="#">规章制度</a></li>
                <li><a href="#">德育网</a></li>
                <li><a href="#">教研网</a></li>
                <li><a href="#">名师风采</a></li>
                <li><a href="#">高考专栏</a></li>
                <li><a href="#">图书馆</a></li>
                <li><a href="#">校友会</a></li>
                <li><a href="#">河中论坛</a></li>
                <li><a href="#">查询系统</a></li>
                <li><a href="#" class="specil">东校区</a></li>     -->                
            </ul>
        </div>           
    </div>
  <div id="dh">
        	<h1><a href="index.html">河北中学首页</a> - <a href="list.html">学校概况</a> - <a href="#">校园文化</a></h1>
        	<div id="search">
        <input name="search" type="text" class="search_text" /><input name="searchbut" type="button" class="search_but" value=" " />
        </div>
      </div>
    <div id="left">
    	<div id="hot">
        	<h2></h2>
            <ul>
		<!-- 推荐热点在后台没有设置栏目等没办法动态实现 -->
            	<li><a href="#">我校举行五四表彰大会暨成人仪式</a></li> 
				<li><a href="#">河北中学4月份家长开放日公告</a> </li>
				<li><a href="#">教育处组织学生收看《2013年中小学… </a></li>
				<li><a href="#">高一年级励志踏青活动花絮 </a></li>
				<li><a href="#">我校组织高一年级励志踏青活动</a></li>
				<li><a href="#">我校举行五四表彰大会暨成人仪式</a></li> 
				<li><a href="#">河北中学4月份家长开放日公告</a></li> 
				<li><a href="#">教育处组织学生收看《2013年中小学…</a></li>
            </ul>
        </div>
      	<div id="pic">
      		<h1></h1>
           	<div id="colee" >
				<div id="colee1">
                <!-- 内容模块 -->
                {pc:content 
                action="position" 
                <!-- 没有catid不是某一个栏目所以不写这个 -->
                posid="2" num="2" order="listorder DESC"}
                 {loop $data $v}<p> <img src="{$v['thumb']}" width="200" height="150" />{$v['title']}</p>{/loop}
                {/pc}
               
				<!-- <p> <img src="{IMG_PATH}/HBschool/pic.gif" width="200" height="150" />2010-2011年度先进单位</p>
				<p> <img src="{IMG_PATH}/HBschool/pic.gif" width="200" height="150" />2010-2011年度先进单位</p>
				<p> <img src="{IMG_PATH}/HBschool/pic.gif" width="200" height="150" />2010-2011年度先进单位</p>
				<p> <img src="{IMG_PATH}/HBschool/pic.gif" width="200" height="150" />2010-2011年度先进单位</p>
				<p> <img src="{IMG_PATH}/HBschool/pic.gif" width="200" height="150" />2010-2011年度先进单位</p>
				<p> <img src="{IMG_PATH}/HBschool/pic.gif" width="200" height="150" />2010-2011年度先进单位</p> -->
			</div>
			<div id="colee2"></div>
		</div>
    </div>
</div>
<div id="right">
    <h1>{$title}</h1>
    <h2>作者：{$username}&nbsp;&nbsp;&nbsp;&nbsp;    图片来源：本站原创&nbsp;&nbsp;&nbsp;&nbsp;     点击数： <span id="hits"></span>&nbsp;&nbsp;&nbsp;&nbsp;     更新时间：{$updatetime}</h2>
        <!-- <p>2013年4月14日，教育处和高一年级组共同组织了高一年级及高二实验部学生“励志踏青”活动。</p>
		<p>此次“励志踏青”活动，行程约30多华里，历时5个小时。同学们从学校大门南行，左转至燕赵大街直行经历史文化街出南城门过子龙大桥，在南桥头右转进入汊河湿地公园景区，然后向西自由活动到神农庄园停车场集合，沿107国道北行至镇远路右转，到承德街左转北行，经恒山西路返回学校。</p>
		<p><img src="{IMG_PATH}/HBschool/newspic.jpg" width="550px" height="380px"></p>
		<p>同学们在此次活动中展现出学校和班级的良好精神风貌。一路上，校旗班旗迎风招展，队伍整齐，每个人脸上都洋溢着青春的笑容。沿途和景区，随处都可以看到同学们捡拾垃圾的身影，互帮互助的身影。在景区，同学们尽情地拥抱大自然，呼吸着自由的空气，和好朋友合影留念。此次活动使同学们在徒步远行中砥砺了意志品质，于集体踏青时领略了湖光水色。</p>
		<p>此次活动经教育处和高一年级组缜密筹划、精心组织，全体班主任和随队老师的通力配合，在校医校车有利的后勤保障下，获得圆满成功！！</p> -->
        {$content}
    <div class="next"><span class="font_next">上一篇：</span><a href="{$previous_page['url']}">{$previous_page['title']}</a><span class="font_next">下一篇：</span><a href="{$next_page['url']}">{$next_page['title']}</a></div>
  </div>

</div>
<div id="foot">	  
Copyright © 2008－2013 http://www.***.com All Rights Reserved   网站备案：冀ICP备00000000号
</div>
<script language="JavaScript" src="{APP_PATH}api.php?op=count&id={$id}&modelid={$modelid}"></script> Contact GitHub API Training Shop Blog About © 2017 GitHub, Inc. Terms Privacy Security Status Help
