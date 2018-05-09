<template>
  <section class="container">
    <div>
      <h1 class="title">
        Spice's portfolio
      </h1>
      <h2 class="subtitle">
        Thank you for coming !
      </h2>
      <ul class="home-list">
        <li><a href="#profile">Profile</a></li>
        <li><a href="#history">History</a></li>
        <li><a href="#works">Works</a></li>
        <li><a href="#contact">Contact</a></li>
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
              <th>フレームワーク</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Yugo Ogura</td>
              <td>21</td>
              <td>javascript, node.js, PHP, HTML/CSS, SQL</td>
              <td>Vue.js, Angular, Laravel, WordPress</td>
            </tr>
          </tbody>
        </table>
      </div>
    </div>
    <div class="profile-section">
      <h2 id="history">履歴</h2>
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
        <div class="works-detail">sample</div>
        <div class="works-detail">sample</div>
        <div class="works-detail">sample</div>
        <div class="works-detail">sample</div>
      </div>
    </div>
    <div class="profile-section">
      <h2 id="contact">連絡</h2>
      <a href="https://twitter.com/rabspice?lang=ja" target="_blank">twitter</a>
      <a href="https://github.com/Spice-Z" target="_blank">GitHub</a>
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
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  display: block;
  font-weight: 300;
  font-size: 70px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
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
  padding: 20px;
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
  border-radius: 10px;
  margin-bottom: 10px;
  width: 200px;
  height: 200px;
  background: #526488;
}
</style>
