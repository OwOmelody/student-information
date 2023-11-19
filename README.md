# student-information
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<style>
    body {
        margin: 0;
        min-width: 250px;
    }

    * {
        box-sizing: border-box;
    }

    .header {
        background-color: #2571c8;
        padding: 20px 40px;
        color: #fff;
        text-align: center;
        font-size: large;
        margin-top: -25px;
    }

    .header::after {
        content: "";
        display: table;
        clear: both;
    }

    input {
        margin: 0;
        border: none;
        width: 75%;
        padding: 10px;
        float: left;
        font-size: 16px;
    }

    .addBtn {
        padding: 10px;
        width: 25%;
        background: #d9d9d9;
        color: #555;
        float: left;
        text-align: center;
        font-size: 16px;
        cursor: pointer;
        transition: 0.3;
    }

    .addBtn:hover {
        background-color: #bbb;
    }


    ul {
        margin: 0;
        padding: 0;
    }

    ul li {
        cursor: pointer;
        position: relative;
        padding: 12px 8px 12px 40px;
        list-style-type: none;
        background: #eee;
        font-size: 18px;
        transition: 0.2;
    }

    ul li:nth-child(odd) {
        background: #f9f9f9;
    }

    ul li:hover {
        background: #ddd;
    }

    ul li.checked {
        background: #888;
        color: #fff;
        text-decoration: line-through;
    }

    ul li.checked::before {
        content: "V";
        position: absolute;
        top: 10px;
        left: 16px;
    }

    .link {
        width: 25%;
        height: 50px;
        color: #425a75;
        padding: 10px;
        background: #d9d9d9;
        float: left;
        text-align: center;
        font-size: 16px;
        cursor: pointer;
        transition: 0.3;
    }

    .box {
        width: 75%;
        height: 50px;
        position: right;
        margin: 0;
        border: none;
        width: 75%;
        padding: 10px;
        float: left;
        font-size: 16px;
        background: #f6f5f5;
    }

    .txt {
        padding-left: 80px;
        font-size: 20px;
    }

    .link2 {
        width: 120px;
        height: 50px;
        color: #425a75;
        background: #d9d9d9;
        float: left;
        text-align: center;
        margin: 5px 0%;
        font-size: 20px;
        cursor: pointer;
        transition: 0.3;
        border-radius: 12px;
    }

    .link25 {
        width: 110px;
        height: 110px;
        color: #425a75;
        background: rgb(127, 205, 236);
        float: left;
        text-align: center;
        margin: -40px -40px;
        font-size: 25px;
        cursor: pointer;
        transition: 0.3;
        border-radius: 50px;
    }

    .link3 {
        width: 120px;
        height: 50px;
        color: #425a75;
        background: #d9d9d9;
        float: right;
        text-align: center;
        margin: -72px 0%;
        font-size: 20px;
        cursor: pointer;
        transition: 0.3;
        border-radius: 12px;
    }

    #red {
        color: red
    }

    #blue {
        color: rgb(215, 215, 255);
    }
</style>

<body>
    <div id="app">
        <button class="link25" @click="btn">.<p>....Hello</p></button>
    </div>

    <div id="app2">
        <h1 v-if="awesome">
            <div class="header">
                <h1>学生资料(2023-2024)</h1>
                <div>
                    <textarea class="box">Text...</textarea>
                    <button class="link">Click</button>
                </div>
            </div>


            <div id="app" class="header">
                <button class="link2" @click="btn">noting here</button>
            </div>


            <div id="app2">
                <div class="header"><button class="link3" @click="toggle">简转繁</button></div>

                <ul>
                    <li>
                        <h2>目录 :</h2>
                    </li>
                    <div class="txt"><a href="#aa">
                            <h2>1).个人履历</h2>
                        </a></div>
                    <div class="txt"><a href="#bb">
                            <h2>2).成绩表副本</h2>
                        </a></div>
                    <div class="txt"><a href="#cc">
                            <h2>3).专业认证副本</h2>
                        </a></div>
                    <div class="txt"><a href="#dd">
                            <h2>4).奖项证明副本</h2>
                        </a></div>
                </ul>

                <ul>
                    <div id="aa">
                        <li>
                            <h2>個人履歷 :</h2>
                        </li>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%80%8B%E4%BA%BA%E5%B1%A5%E6%AD%B7(%E7%B2%BE%E7%B0%A1%E7%89%88).pdf">-个人履历(精简版)
                            </a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%80%8B%E4%BA%BA%E5%B1%A5%E6%AD%B7(%E8%A9%B3%E7%B4%B0%E7%89%88).pdf">-个人履历(详细版)</a>
                        </h2>
                    </div>
                </ul>

                <ul>
                    <div id="bb">
                        <li>
                            <h2>成绩表副本 :</h2>
                        </li>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E8%81%96%E4%BF%9D%E7%A5%BF%E5%AD%B8%E6%A0%A1%E9%AB%98%E4%B8%80%E4%BA%8C%E7%B4%9A%E6%88%90%E7%B8%BE%E8%A1%A8.pdf">-圣保禄学校高一二级成绩表</a>
                        </h2>
                    </div>
                </ul>

                <ul>
                    <div id="cc">
                        <li>
                            <h2>专业认证副本 :</h2>
                        </li>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20Microsoft%20%E8%AA%8D%E8%AD%89Excel%202019%20Associate%E8%AD%89%E6%9B%B8.pdf">-2023年
                                Microsoft 认证Excel 2019 Associate证书</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20Microsoft%20%E8%AA%8D%E8%AD%89PowerPoint%202019%20Associate%E8%AD%89%E6%9B%B8.pdf">-2023年
                                Microsoft 认证PowerPoint 2019 Associate证书</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20Microsoft%20%E8%AA%8D%E8%AD%89PowerPoint%202016%20Associate%E8%AD%89%E6%9B%B8.pdf">-2023年
                                Microsoft 认证PowerPoint 2016 Associate证书</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E7%AC%AC%E5%8D%81%E4%BA%94%E5%B1%86%E6%BE%B3%E9%96%80%E5%AD%B8%E7%94%9FOffice%E8%BB%9F%E4%BB%B6%E6%8A%80%E8%83%BD%E6%AF%94%E8%B3%BD%E7%B6%B2%E4%B8%8A%E5%BC%B7%E5%8C%96%E5%9F%B9%E8%A8%93%E7%8F%AD-POWERPOINT%E8%AD%89%E6%9B%B8.pdf">-2023年
                                第十五届澳门学生Office软件技能比赛网上强化培训班-POWERPOINT证书</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E4%B8%AD%E5%8D%8E%E9%9D%92%E5%B9%B4%E8%BF%9B%E6%AD%A5%E5%8D%8F%E4%BC%9A%20%E7%9F%AD%E8%A7%86%E9%A2%91%E5%88%9B%E4%BD%9C%E5%9F%B9%E8%AE%AD%E7%8F%AD%E6%AF%95%E4%B8%9A%E8%AF%81%E4%B9%A6.pdf">-2023年
                                中华青年进步协会 短片创作训练班毕业证书</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20English%20ambassador%20certificate%20of%20completion.pdf">-2023年
                                English ambassador certificate of completion</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2022%E5%B9%B4%20%E6%98%8E%E6%97%A5%E4%B9%8B%E6%98%9F%E5%BB%A3%E5%91%8A%E7%AD%96%E5%8A%83%E5%9F%B9%E8%A8%93%E8%A8%88%E5%8A%83%E7%95%A2%E6%A5%AD%E8%AD%89%E6%9B%B8.pdf">-2022年
                                明日之星广告策划培训计划毕业证书</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2022%E5%B9%B4%20%E9%9D%92%E5%B9%B4%E7%BE%A9%E5%B7%A5%E5%9F%BA%E7%A4%8E%E5%9F%B9%E8%A8%93%E8%AA%B2%E7%A8%8B(12%E5%B0%8F%E6%99%82)%20%E4%BF%AE%E7%95%A2%E8%AD%89%E6%98%8E%E6%9B%B8.pdf">-2022年
                                青年义工基础培训课程(12小时) 修毕证明书</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2020%E5%B9%B4%202020%E6%88%90%E4%BA%BA%E5%AE%A3%E8%AA%93%E6%97%A5%E6%9B%81%E6%98%8E%E6%97%A5%E9%9D%92%E5%B9%B4%E9%A0%98%E8%A2%96%E5%9F%B9%E8%A8%93%E8%A8%88%E5%8A%83%E5%8F%83%E8%88%87%E5%8F%8A%E5%87%BA%E5%B8%AD%E8%AD%89%E6%9B%B8.pdf">-2020年
                                2020成人宣誓日曁明日青年领袖培训计划参与及出席证书</a></h2>
                    </div>
                </ul>

                <ul>
                    <div id="dd">
                        <li>
                            <h2>奖项证明副本 :</h2>
                        </li>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E6%BE%B3%E9%96%80%E7%89%B9%E5%88%A5%E8%A1%8C%E6%94%BF%E5%8D%80%E6%B5%B7%E9%97%9C%E3%80%8C%E7%A4%BE%E5%8D%80%E6%89%93%E5%81%87%E8%81%AF%E7%B5%A1%E6%A9%9F%E5%88%B6%E3%80%8D%E6%88%90%E7%AB%8B%E4%B8%83%E5%91%A8%E5%B9%B4%E5%9B%9B%E6%A0%BC%E6%BC%AB%E7%95%AB%E6%AF%94%E8%B3%BD.pdf">-2023年
                                澳门特别行政区海关「社区打假联络机制」成立七周年四格漫画比赛</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E4%B8%AD%E8%8F%AF%E5%82%B3%E7%B5%B1%E6%96%87%E5%8C%96%E6%8E%A8%E5%BB%A3%E8%A8%88%E7%95%AB%E9%9D%92%E5%B0%91%E5%B9%B4%E5%89%B5%E6%96%B0%E6%89%8B%E7%B9%AA%E4%B8%AD%E8%8F%AF%E6%96%87%E5%8C%96%E7%89%B9%E8%89%B2%E5%8F%A3%E7%BD%A9%E5%89%B5%E4%BD%9C%E6%AF%94%E8%B3%BD2-%E8%8F%AF%E8%97%9D%E9%A2%A8%E8%B2%8C%E4%B8%AD%E5%AD%B8%E7%B5%84%20%E5%AD%A3%E8%BB%8D.pdf">-2023年
                                中华传统文化推广计画青少年创新手绘中华文化特色口罩创作比赛2-华艺风貌中学组 季军</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E3%80%8C%E8%AD%A6%E5%AF%9F%EF%BC%8E%E5%BD%A2%E8%B1%A1%E3%80%8D%E5%A1%AB%E8%89%B2%E3%80%81%E7%B9%AA%E7%95%AB%E5%8F%8A%E5%8F%A3%E8%99%9F%E6%AF%94%E8%B3%BD%20%E4%B8%89%E7%AD%89%E7%8D%8E.pdf">-2023年
                                「警察．形象」填色、绘画及口号比赛 三等奖</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E3%80%8C%E8%AD%A6%E5%AF%9F%EF%BC%8E%E5%BD%A2%E8%B1%A1%E3%80%8D%E5%A1%AB%E8%89%B2%E3%80%81%E7%B9%AA%E7%95%AB%E5%8F%8A%E5%8F%A3%E8%99%9F%E6%AF%94%E8%B3%BD%20%E5%85%A5%E5%9C%8D%E7%8D%8E.pdf">-2023年
                                「警察．形象」填色、绘画及口号比赛 入围奖</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E6%BE%B3%E9%96%80%E8%81%96%E4%BF%9D%E7%A5%BF%E5%AD%B8%E6%A0%A1%E6%A0%A1%E5%8F%8B%E7%8D%8E%E5%AD%B8%E9%87%91%20FRA%20ANGELICO%E5%AE%89%E5%90%89%E5%88%A9%E7%A7%91%E8%97%9D%E8%A1%93%E7%8D%8E.pdf">-2023年
                                澳门圣保禄学校校友奖学金 FRA ANGELICO安吉利科艺术奖</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20Superior%20Culture%E4%B8%8A%E2%80%A7%E6%96%87%E5%8C%96%E7%9A%84%E5%91%A8%E5%B9%B4%E7%B9%AA%E7%95%AB%E5%A4%A7%E8%B3%BD2023%E5%86%A0%E8%BB%8D.pdf">-2023年
                                Superior Culture上‧文化的周年绘画大赛2023冠军</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20Superior%20Culture%20%E4%B8%8A%E2%80%A7%E6%96%87%E5%8C%96%E7%9A%84%E9%BB%91%E7%99%BD%E7%B9%AA%E7%95%AB%E5%A4%A7%E8%B3%BD2023%E4%BA%9E%E8%BB%8D.pdf">-2023年
                                Superior Culture 上‧文化的黑白绘画大赛2023亚军</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2022%E5%B9%B4%20%E6%BE%B3%E9%96%80%E7%84%A1%E7%96%86%E7%95%8C%E9%9D%92%E5%B9%B4%E5%8D%94%E6%9C%83%20%E7%9A%84%E6%93%81%E6%8A%B1%E3%80%8C%E5%9F%BA%E6%9C%AC%E6%B3%95%E3%80%8D%E6%8A%B1%E6%9E%95%E7%B9%AA%E7%95%AB%E6%AF%94%E8%B3%BD%20%E5%AD%A3%E8%BB%8D.pdf">-2022
                                澳门无疆界青年协会 的拥抱「基本法」抱枕绘画比赛 季军</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2022%E5%B9%B4%20%E3%80%8C%E5%A4%A2%E6%83%B3%E7%AB%A5%E7%9B%9F%E3%80%8D%E7%9A%84%E6%96%B0%E6%98%A5%E5%88%A9%E6%98%AF%E5%B0%81%E8%A8%AD%E8%A8%88%E6%AF%94%E8%B3%BD%20%E5%85%A5%E5%9C%8D%E7%8D%8E.pdf">-2022
                                年 「梦想童盟」的新春利是封设计比赛 入围奖</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2022%E5%B9%B4%20%E3%80%8A%E6%AE%98%E7%96%BE%E4%BA%BA%E6%AC%8A%E5%88%A9%E5%85%AC%E7%B4%84%E3%80%8B%E5%A1%AB%E8%89%B2%E6%AF%94%E8%B3%BD2022%E5%84%AA%E7%95%B0%E7%8D%8E.pdf">-2022年
                                《残疾人权利公约》填色比赛2022优异奖</a></h2>
                    </div>
                    <div class="txt">
                        <h2><a
                                href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2021%E5%B9%B4%20%E8%81%96%E4%BF%9D%E7%A5%BF%E5%AD%B8%E6%A0%A1%E4%BF%9D%E7%A5%BF%E7%B2%BE%E7%A5%9E%E7%8D%8E%E5%8B%B5%E8%A8%88%E5%8A%83%20%E7%8D%8E%E7%8B%80.pdf">-2021年
                                圣保禄学校保禄精神奖励计画 奖状</a></h2>
                    </div>
                </ul>
            </div>
        </h1>

        <h1 v-if="!awesome">
            <div>
                <div class="header">
                    <h1>學生資料(2023-2024)</h1>
                    <div>
                        <textarea class="box">Text...</textarea>
                        <button class="link">Click</button>
                    </div>
                </div>

                <div class="header">
                    <div id="app">
                        <button class="link2" @click="btn">noting here</button>
                    </div>
                </div>

                <div id="app2">
                    <div class="header"><button class="link3" @click="toggle">繁轉簡</button></div>

                    <ul>
                        <li>
                            <h2>目錄 :</h2>
                        </li>
                        <div class="txt"><a href="#aa">
                                <h2>1).個人履歷</h2>
                            </a></div>
                        <div class="txt"><a href="#bb">
                                <h2>2).成績表副本</h2>
                            </a></div>
                        <div class="txt"><a href="#cc">
                                <h2>3).專業認證副本</h2>
                            </a></div>
                        <div class="txt"><a href="#dd">
                                <h2>4).獎項證明副本</h2>
                            </a></div>
                    </ul>

                    <ul>
                        <div id="aa">
                            <li>
                                <h2>個人履歷 :</h2>
                            </li>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%80%8B%E4%BA%BA%E5%B1%A5%E6%AD%B7(%E7%B2%BE%E7%B0%A1%E7%89%88).pdf">-個人履歷(精簡版)</a>
                            </h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%80%8B%E4%BA%BA%E5%B1%A5%E6%AD%B7(%E8%A9%B3%E7%B4%B0%E7%89%88).pdf">-個人履歷(詳細版)</a>
                            </h2>
                        </div>
                    </ul>

                    <ul>
                        <div id="bb">
                            <li>
                                <h2>成績表副本 :</h2>
                            </li>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E8%81%96%E4%BF%9D%E7%A5%BF%E5%AD%B8%E6%A0%A1%E9%AB%98%E4%B8%80%E4%BA%8C%E7%B4%9A%E6%88%90%E7%B8%BE%E8%A1%A8.pdf">-聖保祿學校高一二級成績表</a>
                            </h2>
                        </div>
                    </ul>

                    <ul>
                        <div id="cc">
                            <li>
                                <h2>專業認證副本 :</h2>
                            </li>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20Microsoft%20%E8%AA%8D%E8%AD%89Excel%202019%20Associate%E8%AD%89%E6%9B%B8.pdf">-2023年
                                    Microsoft 認證Excel 2019 Associate證書</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20Microsoft%20%E8%AA%8D%E8%AD%89PowerPoint%202019%20Associate%E8%AD%89%E6%9B%B8.pdf">-2023年
                                    Microsoft 認證PowerPoint 2019 Associate證書</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20Microsoft%20%E8%AA%8D%E8%AD%89PowerPoint%202016%20Associate%E8%AD%89%E6%9B%B8.pdf">-2023年
                                    Microsoft 認證PowerPoint 2016 Associate證書</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E7%AC%AC%E5%8D%81%E4%BA%94%E5%B1%86%E6%BE%B3%E9%96%80%E5%AD%B8%E7%94%9FOffice%E8%BB%9F%E4%BB%B6%E6%8A%80%E8%83%BD%E6%AF%94%E8%B3%BD%E7%B6%B2%E4%B8%8A%E5%BC%B7%E5%8C%96%E5%9F%B9%E8%A8%93%E7%8F%AD-POWERPOINT%E8%AD%89%E6%9B%B8.pdf">-2023年
                                    第十五屆澳門學生Office軟件技能比賽網上強化培訓班-POWERPOINT證書</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E4%B8%AD%E5%8D%8E%E9%9D%92%E5%B9%B4%E8%BF%9B%E6%AD%A5%E5%8D%8F%E4%BC%9A%20%E7%9F%AD%E8%A7%86%E9%A2%91%E5%88%9B%E4%BD%9C%E5%9F%B9%E8%AE%AD%E7%8F%AD%E6%AF%95%E4%B8%9A%E8%AF%81%E4%B9%A6.pdf">-2023年
                                    中華青年進步協會 短片創作訓練班畢業證書</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20English%20ambassador%20certificate%20of%20completion.pdf">-2023年
                                    English ambassador certificate of completion</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2022%E5%B9%B4%20%E6%98%8E%E6%97%A5%E4%B9%8B%E6%98%9F%E5%BB%A3%E5%91%8A%E7%AD%96%E5%8A%83%E5%9F%B9%E8%A8%93%E8%A8%88%E5%8A%83%E7%95%A2%E6%A5%AD%E8%AD%89%E6%9B%B8.pdf">-2022年
                                    明日之星廣告策劃培訓計劃畢業證書</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2022%E5%B9%B4%20%E9%9D%92%E5%B9%B4%E7%BE%A9%E5%B7%A5%E5%9F%BA%E7%A4%8E%E5%9F%B9%E8%A8%93%E8%AA%B2%E7%A8%8B(12%E5%B0%8F%E6%99%82)%20%E4%BF%AE%E7%95%A2%E8%AD%89%E6%98%8E%E6%9B%B8.pdf">-2022年
                                    青年義工基礎培訓課程(12小時) 修畢證明書</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E5%B0%88%E6%A5%AD%E8%AA%8D%E8%AD%89%E5%89%AF%E6%9C%AC/2020%E5%B9%B4%202020%E6%88%90%E4%BA%BA%E5%AE%A3%E8%AA%93%E6%97%A5%E6%9B%81%E6%98%8E%E6%97%A5%E9%9D%92%E5%B9%B4%E9%A0%98%E8%A2%96%E5%9F%B9%E8%A8%93%E8%A8%88%E5%8A%83%E5%8F%83%E8%88%87%E5%8F%8A%E5%87%BA%E5%B8%AD%E8%AD%89%E6%9B%B8.pdf">-2020年
                                    2020成人宣誓日曁明日青年領袖培訓計劃參與及出席證書</a></h2>
                        </div>
                    </ul>

                    <ul>
                        <div id="dd">
                            <li>
                                <h2>獎項證明副本 :</h2>
                            </li>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E6%BE%B3%E9%96%80%E7%89%B9%E5%88%A5%E8%A1%8C%E6%94%BF%E5%8D%80%E6%B5%B7%E9%97%9C%E3%80%8C%E7%A4%BE%E5%8D%80%E6%89%93%E5%81%87%E8%81%AF%E7%B5%A1%E6%A9%9F%E5%88%B6%E3%80%8D%E6%88%90%E7%AB%8B%E4%B8%83%E5%91%A8%E5%B9%B4%E5%9B%9B%E6%A0%BC%E6%BC%AB%E7%95%AB%E6%AF%94%E8%B3%BD.pdf">-2023年
                                    澳門特別行政區海關「社區打假聯絡機制」成立七周年四格漫畫比賽</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E4%B8%AD%E8%8F%AF%E5%82%B3%E7%B5%B1%E6%96%87%E5%8C%96%E6%8E%A8%E5%BB%A3%E8%A8%88%E7%95%AB%E9%9D%92%E5%B0%91%E5%B9%B4%E5%89%B5%E6%96%B0%E6%89%8B%E7%B9%AA%E4%B8%AD%E8%8F%AF%E6%96%87%E5%8C%96%E7%89%B9%E8%89%B2%E5%8F%A3%E7%BD%A9%E5%89%B5%E4%BD%9C%E6%AF%94%E8%B3%BD2-%E8%8F%AF%E8%97%9D%E9%A2%A8%E8%B2%8C%E4%B8%AD%E5%AD%B8%E7%B5%84%20%E5%AD%A3%E8%BB%8D.pdf">-2023年
                                    中華傳統文化推廣計畫青少年創新手繪中華文化特色口罩創作比賽2-華藝風貌中學組 季軍</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E3%80%8C%E8%AD%A6%E5%AF%9F%EF%BC%8E%E5%BD%A2%E8%B1%A1%E3%80%8D%E5%A1%AB%E8%89%B2%E3%80%81%E7%B9%AA%E7%95%AB%E5%8F%8A%E5%8F%A3%E8%99%9F%E6%AF%94%E8%B3%BD%20%E4%B8%89%E7%AD%89%E7%8D%8E.pdf">-2023年
                                    「警察．形象」填色、繪畫及口號比賽 三等獎</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E3%80%8C%E8%AD%A6%E5%AF%9F%EF%BC%8E%E5%BD%A2%E8%B1%A1%E3%80%8D%E5%A1%AB%E8%89%B2%E3%80%81%E7%B9%AA%E7%95%AB%E5%8F%8A%E5%8F%A3%E8%99%9F%E6%AF%94%E8%B3%BD%20%E5%85%A5%E5%9C%8D%E7%8D%8E.pdf">-2023年
                                    「警察．形象」填色、繪畫及口號比賽 入圍獎</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20%E6%BE%B3%E9%96%80%E8%81%96%E4%BF%9D%E7%A5%BF%E5%AD%B8%E6%A0%A1%E6%A0%A1%E5%8F%8B%E7%8D%8E%E5%AD%B8%E9%87%91%20FRA%20ANGELICO%E5%AE%89%E5%90%89%E5%88%A9%E7%A7%91%E8%97%9D%E8%A1%93%E7%8D%8E.pdf">-2023年
                                    澳門聖保祿學校校友獎學金 FRA ANGELICO安吉利科藝術獎</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20Superior%20Culture%E4%B8%8A%E2%80%A7%E6%96%87%E5%8C%96%E7%9A%84%E5%91%A8%E5%B9%B4%E7%B9%AA%E7%95%AB%E5%A4%A7%E8%B3%BD2023%E5%86%A0%E8%BB%8D.pdf">-2023年
                                    Superior Culture上‧文化的周年繪畫大賽2023冠軍</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2023%E5%B9%B4%20Superior%20Culture%20%E4%B8%8A%E2%80%A7%E6%96%87%E5%8C%96%E7%9A%84%E9%BB%91%E7%99%BD%E7%B9%AA%E7%95%AB%E5%A4%A7%E8%B3%BD2023%E4%BA%9E%E8%BB%8D.pdf">-2023年
                                    Superior Culture 上‧文化的黑白繪畫大賽2023亞軍</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2022%E5%B9%B4%20%E6%BE%B3%E9%96%80%E7%84%A1%E7%96%86%E7%95%8C%E9%9D%92%E5%B9%B4%E5%8D%94%E6%9C%83%20%E7%9A%84%E6%93%81%E6%8A%B1%E3%80%8C%E5%9F%BA%E6%9C%AC%E6%B3%95%E3%80%8D%E6%8A%B1%E6%9E%95%E7%B9%AA%E7%95%AB%E6%AF%94%E8%B3%BD%20%E5%AD%A3%E8%BB%8D.pdf">-2022
                                    澳門無疆界青年協會 的擁抱「基本法」抱枕繪畫比賽 季軍</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2022%E5%B9%B4%20%E3%80%8C%E5%A4%A2%E6%83%B3%E7%AB%A5%E7%9B%9F%E3%80%8D%E7%9A%84%E6%96%B0%E6%98%A5%E5%88%A9%E6%98%AF%E5%B0%81%E8%A8%AD%E8%A8%88%E6%AF%94%E8%B3%BD%20%E5%85%A5%E5%9C%8D%E7%8D%8E.pdf">-2022
                                    年 「夢想童盟」的新春利是封設計比賽 入圍獎</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2022%E5%B9%B4%20%E3%80%8A%E6%AE%98%E7%96%BE%E4%BA%BA%E6%AC%8A%E5%88%A9%E5%85%AC%E7%B4%84%E3%80%8B%E5%A1%AB%E8%89%B2%E6%AF%94%E8%B3%BD2022%E5%84%AA%E7%95%B0%E7%8D%8E.pdf">-2022年
                                    《殘疾人權利公約》填色比賽2022優異獎</a></h2>
                        </div>
                        <div class="txt">
                            <h2><a
                                    href="file:///C:/Users/s56022/Desktop/%E5%AD%B8%E7%94%9F%E8%B3%87%E6%96%99/%E7%8D%8E%E9%A0%85%E8%AD%89%E6%98%8E%E5%89%AF%E6%9C%AC/2021%E5%B9%B4%20%E8%81%96%E4%BF%9D%E7%A5%BF%E5%AD%B8%E6%A0%A1%E4%BF%9D%E7%A5%BF%E7%B2%BE%E7%A5%9E%E7%8D%8E%E5%8B%B5%E8%A8%88%E5%8A%83%20%E7%8D%8E%E7%8B%80.pdf">-2021年
                                    聖保祿學校保祿精神獎勵計畫 獎狀</a></h2>
                        </div>
                    </ul>
                </div>
        </h1>
    </div>


    <script type="module">

        import { createApp, ref } from 'https://unpkg.com/vue@3/dist/vue.esm-browser.js'

        const app = createApp({
            data() {
                return {
                    txt: 'blue'
                }
            },
            methods: {
                btn() { alert('Nice to meet you') }
            }
        })

        app.mount('#app')
    </script>

    <script type="module">

        import { createApp, ref } from 'https://unpkg.com/vue@3/dist/vue.esm-browser.js'

        const app2 = createApp({
            data() {
                return {
                    awesome: true
                }
            },
            methods: {
                toggle() { this.awesome = !this.awesome }
            }
        })

        app2.mount('#app2')
    </script>

</body>

</html>
