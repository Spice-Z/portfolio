<template>
  <section class="container">
    <div class="head-section">
      <div class="title-container">
        <h1 class="title">
          Spice's portfolio
        </h1>
        <h2 class="subtitle">
          Thank you for coming !
        </h2>
      </div>
      <ul class="home-list">
        <li><a href="#profile">Profile</a></li>
        <li><a href="#history">History</a></li>
        <li><a href="#works">Works</a></li>
        <li><a href="#contact">Acount</a></li>
      </ul>
    </div>
    <div class="profile-section">
      <h2 id="profile">自己紹介</h2>
      <div class="profile-box">
        <img src="../assets/githubIcon.jpeg" alt="">
        <div class="profile-sentences">
          <p>
            はじめまして。すぱいすです。<br>
            大学1年生で始めてプログラミングに触れ、その後、独学で勉強をしてきました。<br>
            今は、名古屋の会社でフロントエンドエンジニアとしてアルバイトをしています。<br>
            卒業後は東京の会社に就職予定です。
          </p>
        </div>
      </div>
      <div class="table-container">
        <table class="profile-table">
          <thead>
            <tr>
              <th>Name</th>
              <th>Age</th>
              <th>使用言語</th>
              <th>ライブラリ・フレームワーク</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Yugo Ogura</td>
              <td>21</td>
              <td>javascript, node.js, PHP, HTML/CSS, SQL</td>
              <td>Vue.js, Nuxt.js, Angular, express, Laravel, WordPress etc...</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
    <div class="profile-section">
      <h2 id="history">開発履歴</h2>
      <div class="history-box">
        <div class="history-line"></div>
        <div class="history-detail-box">
          <div class="history-detail"><span class="history-detail-title">2015/04</span> 大学の講義で初めてプログラミング(C言語)に触れる</div>
          <div class="history-detail"><span class="history-detail-title">2015/08</span> サークルにてPHP(WordPress)を始めて触り、勉強を始める</div>
          <div class="history-detail"><span class="history-detail-title">2017/01</span> 株式会社ヒットラインにて、エンジニアとしてアルバイトを始める</div>
          <div class="history-detail"><span class="history-detail-title">2017/08,09</span> 株式会社LITALICO, 株式会社エウレカにてサマーインターン</div>
          <div class="history-detail"><span class="history-detail-title">2018/05</span> 株式会社エイチーム引っ越し侍にて、フロントエンドエンジニアとしてアルバイトを始める</div>
        </div>
        
      </div>
    </div>
    <div class="profile-section">
      <h2 id="works">作成物</h2>
      <div class="works-box">
        <div class="works-detail work-detail-portfolio"></div>
        <div class="works-detail work-detail-dockhack"></div>
        <div class="works-detail work-detail-cancamp"></div>
        <div class="works-detail">Admin Menu</div>
      </div>
    </div>
    <div class="profile-section">
      <h2 id="contact">アカウント</h2>
      <a href="https://twitter.com/rabspice?lang=ja" target="_blank">twitter</a>
      <br>
      <a href="https://github.com/Spice-Z" target="_blank">GitHub</a>
      <br>
      <a href="https://qiita.com/spice" target="_blank">Qiita</a>
    </div>
  </section>
</template>

<script>
import AppLogo from "~/components/AppLogo.vue";

export default {
  components: {
    AppLogo
  }
};
</script>

<style>
.container {
  padding: 0;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.head-section {
  width: 100%;
  position: relative;
}

.title-container::before {
  z-index: -1;
  display: block;
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  content: "";
  background: url("../assets/header-background.jpg");
  background-size: cover;
  filter: grayscale(80%) blur(3px);
}

.title-container {
  z-index: 100;
  position: relative;
  padding-top: 100px;
  padding-bottom: 100px;
  width: 100%;
  overflow: hidden;
}

.title {
  display: block;
  font-weight: 300;
  font-size: 70px;
  color: #fdffec;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #fdffec;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

.home-list li {
  display: inline-block;
  padding: 25px;
}

.profile-section {
  margin-top: 20px;
  padding: 0 30px 0 30px;
  width: 100%;
}

.profile-box {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

.profile-box img {
  width: 200px;
  height: 200px;
  border-radius: 50%;
}

.profile-sentences {
  padding: 20px 0;
  text-align: left;
}

.table-container {
  margin-left: 10px;
  margin-right: 10px;
  min-width: 300px;
  overflow-x: scroll;
}

.profile-table {
  min-width: 785px;
}

.history-box {
  display: flex;
  flex-wrap: wrap;
  width: 100%;
}

.history-line {
  border-radius: 5px;
  width: 10px;
  background: #9055c4;
}

.history-detail-box {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  max-width: 95%;
}

.history-detail {
  position: relative;
  margin-bottom: 20px;
  padding-left: 15px;
  text-align: left;
}

.history-detail-title {
  font-weight: 700;
}

.history-detail::before {
  display: inline-block;
  position: absolute;
  left: -20px;
  margin-top: 6px;
  content: "";
  border-radius: 50%;
  background: #ffffff;
  width: 30px;
  height: 30px;
  border: solid 10px #9055c4;
}

.works-box {
  display: inline-flex;
  flex-wrap: wrap;
  justify-content: space-around;
  width: 100%;
}

.works-detail {
  position: relative;
  border-radius: 10px;
  margin-bottom: 20px;
  width: 250px;
  height: 250px;
  text-align: center;
  line-height: 240px;
}

.works-detail::before {
  content: "";
  display: block;
  position: absolute;
  z-index: -1;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  border-radius: 10px;
  box-shadow: 0 2px 8px 3px rgba(0, 0, 0, 0.5);
}

.work-detail-portfolio::before {
  background: url("../assets/portfolio.png");
  background-size: cover;
  background-position: center top;
  filter: grayscale(10%);
}

.work-detail-dockhack::before {
  background: url("../assets/dockhack.png");
  background-size: cover;
  background-position: center top;
  filter: grayscale(20%);
}

.work-detail-cancamp::before {
  background: url("../assets/cancamp.jpg");
  background-size: cover;
  background-position: center;
  filter: grayscale(20%);
}
</style>
