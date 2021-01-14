<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>geek网页复现</title>
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>
    <!--第一个大背景以及用来包括此背景中的各个元素-->
    <div id="bk">
      <!--固定定位在网页顶部的导航栏-->
      <div id="uper">
        <!--为了使五个盒子整齐排列在一行，将这五个盒子转化为行内块元素-->
        <div class="hang_nei_kuai">
          <!--使用锚点链接，与之后做的各个专题模块对应建立链接-->
          <a href="#about_us">
            <!--这里的类都共同使用一个样式，但是对于部分位置再单独使用其他样式进行微调-->
            <span class="text_style about">About Us</span>
          </a>
        </div>
        <div class="hang_nei_kuai">
          <a href="#introduction">
            <span class="text_style">Introduction</span>
          </a>
        </div>
        <div class="hang_nei_kuai">
          <a href="https://new-thread.com//">
            <span class="text_style newthread">NewThread</span>
          </a>
        </div>
        <div class="hang_nei_kuai">
          <a href="#more_question">
            <span class="text_style Q">Q&Ask</span>
          </a>
        </div>
        <div class="hang_nei_kuai contact">
          <a href="#contactus">
            <span class="text_style">Contact Us</span>
          </a>
        </div>
      </div>
      <!--为了使得GEEK图片在较下的位置，在这个图片的上方放一个行内元素，利用css转化为块元素，以此来调整GEEK图片的位置
        （其实直接使用一个块元素也可以）-->
      <span id="GK_up"></span>
      <!--GEEK的大图片，将要做成一个有动画效果的图片-->
      <div class="img_GK">
        <img
          src="https://gitee.com/gritandsea/picture/raw/master/img/GK.png"
          width="520px"
          height="215px"
          class="animation"
        />
      </div>
      <div class="GK_bottom">
        &nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Keep Curiosity
        <br />
        The Power Of Change
      </div>
    </div>
    <!--尝试双层背景图片叠加完成introduction的大标题部分-->
    <!--这个大盒子设置introduction旁边的两个装饰物-->
    <div class="bk_introduction">
      <!--这个盒子的背景图片放上introduction，之后使得这个位置和固定定位的导航栏的introduction选项之间构建起链接-->
      <div class="img_introduction" id="introduction"></div>
    </div>
    <!--开发程序猿整个界面的大盒子-->
    <div class="total_style">
      <!--里面先放两个小盒子，转成行内块元素，并排摆放-->
      <div class="text_of_programmer">
        <!--这三个盒子放左部分的各种文字，行间距较大但是却小于一个字的高度的都是一个独立的盒子，单独设置了盒子的外边距或者内边距-->
        <p class="programmer1">"开发程序猿"</p>
        <br />
        <p class="programmer2">“Stay Hungry，Stay Foolish”</p>
        <br />
        <p class="programmer3">
          前端:前端开发是创建Web或app视觉界面呈现给用户的过程通过HTML，CSS及JavaScript以及衍生出来的各种技术、框架、解决方案，实现互联网产品的用户界面交互。
        </p>
        <br />
        <p class="programmer3">
          后端:通常也称服务器端开发。不对用户显示,负责处理前端的请求，进行逻辑处理和数据交互。
        </p>
        <br />
        <p class="programmer3">
          客户端:移动应用开发是为了小型、无线计算设备编写软件的流程和程序的集合，例如智能手机或平板电脑。
        </p>
      </div>
      <!--直接使用背景图片，方便调整-->
      <div class="img_monkey"></div>
    </div>
    <!--选择使用盒子来调整盒子之间的距离，而不用外边距margin，因为想要所有大盒子都用一个css样式，因此margin不好控制-->
    <div class="vacancy"></div>
    <!--产品经理的大盒子-->
    <div class="total_style">
      <!--排版，一个照片，另一个装文字的盒子（转为行内块元素）-->
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/chanpin.png"
        width="448px"
        height="550.4px"
        class="img_product"
      />
      <div class="text_of_product">
        <p class="produce1">产品经理/UI设计(PM/UI)</p>
        <br />
        <p class="produce2">"好的软件的特征是,明明没用过,</p>
        <p class="produce2">但总觉得用过似的。"</p>
        <br />
        <p class="produce3">PM是针对某一项或是某一类的产品进行规划和管理的人员。</p>
        <br />
        <p class="produce3">
          PM需要拥有缜密的产品逻辑思维，研究用户心理，负责产品的整个生命周期。
        </p>
        <br />
        <p class="produce3">
          PM参与产品的UI和交互设计，为设计和开发确定产品原型，能够将产品变得有个性,操作变得舒适简单、自由。
        </p>
        <br />
        <p class="produce3">
          PM需要一定的文档能力和沟通能力，能够在团队合作的过程中跟各个角色进行有效沟通。
        </p>
      </div>
    </div>
    <!--选择使用盒子来调整盒子之间的距离，而不用外边距margin，因为想要所有大盒子都用一个css样式，因此margin不好控制-->
    <div class="vacancy1"></div>
    <!--AI算法的大盒子-->
    <div class="total_style">
      <div class="text_of_ai">
        <p class="ai1">AI/算法(AI/AIGO)</p>
        <br />
        <p class="ai2">"路漫漫其修远兮，非大毅力者不能"</p>
        <br />
        <p class="ai3">
          人工智能站在了风口，机器学习和深度学习是它的分支，是团队仍在探索的方向。
        </p>
        <br />
        <p class="ai3">
          当下AI技术的应用涉及到图像处理、自然语言处理、推荐系统和无人驾驶等领域。
        </p>
        <br />
        <p class="ai3">
          AI的核心就是算法和性能。充满科技感的背后，是大量的数学统计理论和计算机知识。
        </p>
      </div>
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/ai.png"
        width="600px"
        height="600px"
        class="img_ai"
      />
    </div>
    <div class="vacancy2"></div>
    <!--安全工程狮的大盒子-->
    <div class="total_style">
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/anquan.png"
        width="500px"
        height="550px"
        class="img_safety"
      />
      <div class="text_of_safety">
        <p class="safety1">安全攻城狮(Sacurity)</p>
        <br />
        <p class="safety2">"我们需要的不是脚本小子，而是对底层原理了如指掌。"</p>
        <br />
        <p class="safety3">
          主要涉及网络攻防、漏洞挖掘，能够代表团队参加CTF安全赛事。
        </p>
        <br />
        <p class="safety3">
          互联网安全从其本质上来讲其实就是互联网上的信息安全。网络安全攻城狮是拥有扎实基础的SuperHacker,同时具有强大的自学能力。
        </p>
        <br />
        <p class="safety3">
          网络安全攻城狮能够识别IT系统的优缺点。并且了解黑客以及网络犯罪手段,且精通网络安全技术:包括服务漏洞扫描、程序漏洞分析检测、病毒木马防范等。
        </p>
      </div>
    </div>
    <div class="vacancy3"></div>
    <!--about us的框架-->
    <!--一共预计使用三个盒子进行框架的搭建-->
      <!--第一个盒子放三个图片-->
      <div class="about_us1">
        <img
          src="https://gitee.com/gritandsea/picture/raw/master/img/左上.png"
          width="153.59px"
          height="48.05px"
          class="img_top_left"
        />
        <img
          src="https://gitee.com/gritandsea/picture/raw/master/img/关于.png"
          width="256px"
          height="80.54px"
          class="img_about_us"
        />
        <img
          src="https://gitee.com/gritandsea/picture/raw/master/img/youshang.png"
          width="153.59px"
          height="48.11px"
          class="img_top_right"
        />
      </div>
      <!--第二个盒子放一个瓢虫和一个蝴蝶，中间有三个圆角边框div盒子-->
      <div class="about_us2">
        <img
          src="https://gitee.com/gritandsea/picture/raw/master/img/七星虫子.png"
          width="115px"
          height="113px"
          class="insect"
        />
        <!--每一个盒子中摆放一个图片以及一个span文本框-->
        <!--这里的三个小盒子首先使用aboutus3进行一个外边框的样式统一，再另外设立类对每一个盒子的位置进行微调-->
        <div class="about_us3 about_us4">
          <img
            src="https://gitee.com/gritandsea/picture/raw/master/img/duoyuan.png"
            width="128px"
            height="167px"
            class="img_diversity"
          />
          <p class="text_of_diversity">
            多元化是我们的特色。在这里，你可以拥有多种方向选择，前后端、安全、AI、算法、产品等。
          </p>
        </div>
        <div class="about_us3 about_us5">
          <img
            src="https://gitee.com/gritandsea/picture/raw/master/img/speech.png"
            width="128px"
            height="166.4px"
            class="img_speech"
          />
          <p class="text_of_speech">
            每周我们会举行一次技术例会，用来汇报我们的学习内容，供成员之间交流学习。
          </p>
        </div>
        <div class="about_us3 about_us6">
          <img
            src="https://gitee.com/gritandsea/picture/raw/master/img/shijian.png"
            width="128px"
            height="166.4px"
            class="img_time"
          />
          <p class="text_of_time">
            耐心、毅力是我们必备的品质，每周我们会至少花30小时在实验室中。以保证技术的精进。
          </p>
        </div>
        <img
          src="https://gitee.com/gritandsea/picture/raw/master/img/hudie.png"
          width="121px"
          height="147px"
          class="img_butterfly"
        />
      </div>
      <!--第三个盒子里面放两个图片-->
      <!--aboutus的bottom就简写为abottom-->
      <div class="abottom">
        <img
          src="https://gitee.com/gritandsea/picture/raw/master/img/左下.png"
          width="153.59px"
          height="51.27px"
        />
        <img
          src="https://gitee.com/gritandsea/picture/raw/master/img/youxia.png"
          width="153.59px"
          height="51.44px"
          class="img_bottom_right"
        />
      </div>
    <!--contact us内容的大盒子-->
    <!--大致构想是分为三块，首先是图片的部分，其次是文字的部分，最后是三个圆角填充的链接-->
    <div class="biggest_contact_us">
      <!--这里是图片模块-->
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/联系我们.png"
        width="307.2px"
        height="79.26px"
        class="img_contact_us"
      />
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/yezi1.png"
        width="128px"
        height="103.63px"
        class="img_leaf"
      />
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/左边的树.png"
        width="307.71px"
        height="486.4px"
        class="img_left_tree"
      />
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/右边的树.png"
        width="422.34px"
        height="550.4px"
        class="img_right_tree"
      />
      <!--放置所有的文字的模块-->
      <div class="frame_of_contact_us1">
        <p class="text_of_contact_us">•热爱计算机，具有geek精神，喜欢DIY，动手能力较强</p>
        <p class="text_of_contact_us">•有编程/算法/硬件基础为佳(有作品可附上)</p>
        <p class="text_of_contact_us">•有足够的空余时间，热爱思考，对事物有自己的见解</p>
        <p class="text_of_contact_us">
          ps:非新思路统招只有通过发送邮件自我介绍后，收到邮件回执后才会被允许进群,在读学生,都可邮件到newthread_geek@outlook.com报名加入.(信中需备注个人基本信息以及意向方向,此招新活动为长期招新)
        </p>
      </div>
      <!--三个圆角填充的链接模块-->
      <div class="frame_of_contact_us2">
        <div class="button_of_contact_us">
          <!--为了使得光标移到图标上以后出现相关的文字提示，可以用a链接加上title（也可以采用button来完成此效果）-->
          <a
            href="https://qm.qq.com/cgi-bin/qm/qr?k=_MXIavH-bKiRMl5LvZHVKnIjjhuHDNGC&jump_from=webapi"
            title="群号：1050679488"
            class="text_of_button_style QQ"
          >
            QQ Group
          </a>
        </div>
        <div class="button_of_contact_us position_of_Email">
          <a href="#" title="newthread-geek@outlook.com" class="text_of_button_style E">
            E-mail
          </a>
        </div>
        <div class="button_of_contact_us position_of_Github">
          <a href="https://github.com/ntgeek" title="Geek组Github" class="text_of_button_style G">
            Github
          </a>
        </div>
      </div>
    </div>
<!--最后一个部分大致分为两个部分，一个是文本部分，一个是图片部分，
  先调好文本居中，再根据图片相对于文本的位置来对图片进行放置-->
    <div class="outer_of_more">
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/question.png"
        width="1011px"
        height="108px"
        class="img_more"
      />
    </div>
    <div class="frame_of_more_img">
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/s.png"
        width="294.4px"
        height="214.94px"
        class="img_s"
      />
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/e.png"
        width="256px"
        height="195.03px"
        class="img_e"
      />
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/白.png"
        width="128px"
        height="94.76px"
        class="img_empty1"
      />
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/白.png"
        width="102.4px"
        height="75.81px"
        class="img_empty2"
      />
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/1.png"
        width="192px"
        height="148.2px"
        class="img_1"
      />
      <img
        src="https://gitee.com/gritandsea/picture/raw/master/img/g.png"
        width="153.59px"
        height="118.55px"
        class="img_g"
      />
<!--最后的一个部分的回收效果，一开始不给盒子中存放回答的高度，并隐藏回答文字。
  通过css3样式控制每一个块的盒子的大小完成展开效果，在此时使得回答显示即可-->
      <div class="text_of_more">
        <!--主要用于包括问题和答案两个部分的元素，便于使用css进行分别的操作-->
        <div id="text_outer_more1">
          <p id="text_title_of_more">1.什么是Geek(极客)？Geek精神又是什么？</p>
          <div id="text_inner_of_more">
            拥有好奇之心，改变之力，爱钻研，能折腾。
          </div>
        </div>
        <div id="text_outer_more2">
          <p id="text_title_of_more">2.招新是安排在什么时间？</p>
          <div id="text_inner_of_more">
            按照惯例，正式招新时间是在9月下旬~10月上旬，不过今年会有一些改动，笔试地点一般在9号教学楼。
            如果想要了解我们，可以加入我们的QQ群，招新具体的安排/变动会在招新群通知。
          </div>
        </div>
        <div id="text_outer_more3">
          <p id="text_title_of_more">3.我们有考核吗？考核流程是怎样的呀？</p>
          <div id="text_inner_of_more">
            嗯...我们一共有一轮笔试和两轮面试。权衡技术、经验和学习能力，
            第一轮是一些视野性的题目，淘汰率并不高。第二轮单独面试，
            根据你的笔试提出技术相关的问题、兴趣爱好、个人看法。最后一轮群面，
            首先问及时间分配上的问题，其次也会向你提出各种奇怪的问题。
            这一轮中许多题目其实并不难，也无标准答案，重在考察同学们在压力下的逻辑思维。
            全部通过成为预备成员啦。
          </div>
        </div>
        <div id="text_outer_more4">
          <p id="text_title_of_more">4.考核是怎样的形式？</p>
          <div id="text_inner_of_more">
            在考核期间每人会拥有一位'长者'带你入门，学习技术与知识，
            交流经验与想法。完成每周的新人任务后再进行一次考核筛选后就可以成为Geek组正式成员啦！
            在考核期必须满足每周30个小时在实验室哦,所以考核期也不可以懈怠哦！
          </div>
        </div>
        <div id="text_outer_more5">
          <p id="text_title_of_more">5.进入Geek组之后都有什么福利呢？</p>
          <div id="text_inner_of_more">
            1对1的新人指引，每一个成员都有会一个mentor,
            带你初入门槛，与你一同成长，组内管理较宽松,
            在尊重其他人的前提下可以尽情发挥自己的个性。
            打破平淡，与同样疯狂的人把疯狂的idea实现，
            磨砺耐性、培养思维、成就梦想。Lab设备/网络资源充足，
            闲暇之余也有组织活动。更有许多的故事等你来听~
          </div>
        </div>
        <div id="text_outer_more6">
          <p id="text_title_of_more">6.进入团队会影响我的日常学习吗？</p>
          <div id="text_inner_of_more">
            你要知道大学是一个可以自由安排自己学习生活的地方。
            如果你想在上课之余充实自己、激励自己，最好的方法就是和比自己更优秀的人在一起。
            团队不缺优秀的人，而我们也期待同样优秀的你，让我们一起前进！
            小组里也有不少保研,考研的前辈们, 大部分都能找到一个平衡点,
            而且团队的经历对你日后读研, 工作都大有裨益。
          </div>
        </div>
        <div id="text_outer_more7">
          <p id="text_title_of_more">7.老师以及学长学姐们的期望是什么?</p>
          <div id="text_inner_of_more">
            我们希望你有很强的自学能力，同时关注新事物、新技术，
            喜欢挑战，逻辑性强，善于和各种文化的人合作.“每个人都可以做自己想做的事情，
            每个人的方向不一样。如果你想做产品或有不错的idea，
            那么就可以找志同道合的人一起合作。”
          </div>
        </div>
      </div>
    </div>
  </body>
</html>
