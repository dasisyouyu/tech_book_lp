<template>
  <section class="container">
    <vs-row vs-w="12">
      <vs-col vs-w="12" vs-type="flex" vs-align="flex-start" vs-justify="flex-start">
        <img class="top_wave" src="~assets/top_wave.svg" alt="top_wave">
      </vs-col>
    </vs-row>

    <vs-row>
      <vs-col vs-w="12" vs-type="flex" vs-justify="center">
        <img src="~assets/title.svg" alt="title">
      </vs-col>

      <vs-col class="fish">
        <img v-parallax="0.3" src="~assets/fish.svg" alt="fish">
      </vs-col>

      <vs-col class="pipico">
        <img v-parallax="0.6" src="~assets/pipico.svg" alt="pipico">
      </vs-col>

      <vs-col vs-offset="2" vs-w="8" vs-type="flex" vs-justify="center">
        <p class="title_content">
          4人での合作です。slackコマンドをGASで作成するチュートリアルとtips たくさん手にとってもらえる技術書の作り方と、得する選び方について<br> イベントイラストのインスピレーションおよび発想の過程について react reduxの最適解。
        </p>
      </vs-col>
    </vs-row>

    <vs-row>
      <vs-col class="tech_books" vs-offset="1" vs-w="10" vs-type="flex" vs-justify="space-around" >
        <div class="tech_book6">
          <img class="book_img" src="~assets/tech_book6.png" alt="tech_book6">
          <img class="new_icon" src="~assets/new_icon.png" alt="new_icon">
          <p class="content_first">
            技術のおつまみ<br>
            redux・design・GAS
          </p>
          <p class="content_second">
            同人誌 / 40ページ / ￥1500
          </p>
        </div>
        <div>
          <img class="book_img" src="~assets/tech_book5.png" alt="tech_book5">
          <p class="content_first">
            nuxtとvuesaxとDjangoで作るモダン<br>
            なサービスの作り方。 tipsもあるよ！
          </p>
          <p class="content_second">
            同人誌 / 28ページ / ￥500 PDF: ￥800
          </p>
        </div>
      </vs-col>
    </vs-row>

    <vs-row class="gallery">
      <vs-col vs-w="12" vs-type="flex" vs-justify="center">
        <h1>GALLERY</h1>
      </vs-col>

      <vs-col vs-w="12" vs-type="flex" vs-justify="center">
        <div class="download_image">
          <img src="~assets/spring.png" alt="spring">
          <vs-chip class="chip" color="danger">spring</vs-chip>
          <a :href="require('~/assets/spring.png')" download>
            <vs-button size="large" color="primary">DOWNLOAD</vs-button>
          </a>
        </div>

        <div class="download_image">
          <img src="~assets/spring.png" alt="spring">
          <vs-chip class="chip" color="danger">spring</vs-chip>
          <a :href="require('~/assets/spring.png')" download>
            <vs-button size="large" color="primary">DOWNLOAD</vs-button>
          </a>
        </div>

        <div class="download_image">
          <img src="~assets/spring.png" alt="spring">
          <vs-chip class="chip" color="danger">spring</vs-chip>
          <a :href="require('~/assets/spring.png')" download>
            <vs-button size="large" color="primary">DOWNLOAD</vs-button>
          </a>
        </div>

        <div class="download_image">
          <img src="~assets/spring.png" alt="spring">
          <vs-chip class="chip" color="danger">spring</vs-chip>
          <a :href="require('~/assets/spring.png')" download>
            <vs-button size="large" color="primary">DOWNLOAD</vs-button>
          </a>
        </div>

        <div class="download_image">
          <img src="~assets/spring.png" alt="spring">
          <vs-chip class="chip" color="danger">spring</vs-chip>
          <a :href="require('~/assets/spring.png')" download>
            <vs-button size="large" color="primary">DOWNLOAD</vs-button>
          </a>
        </div>
      </vs-col>
    </vs-row>
  </section>
</template>

<style lang="scss">
.container {
  min-height: 150vh;
  background-color: #9ad5dc;
  .fish {
    position: absolute;
    img {
      margin-left: 15%;
      width: 10%;
      z-index: 1;
    }
  }
  .pipico {
    position: absolute;
    img {
      margin-left: 85%;
      width: 12%;
      z-index: 1;
    }
  }
  .top_wave {
    width: 100vw;
  }

  .title_content {
    margin-top: 8%;
    text-align: center;
    z-index: 2;
  }

  .tech_books {
    text-align: center;
    margin-top: 8%;
    z-index: 2;
    .book_img {
      width: 80%;
    }
    .new_icon {
      position: absolute;
      left: 10%;
      top: 13%;
      height: 12%;
    }
    .tech_book6 {
      position: relative;
      .book_img {
        position: relative;
      }
    }
    .content_first {
      color: #4a4a4a;
      font-size: 14px;
      font-family: HiraginoSans-W6;
    }
    .content_second {
      color: #ffffff;
      font-family: HiraginoSans-W3;
      font-size: 12px;
    }
  }

  .gallery {
    h1 {
      color: #ffffff;
      font-size: 2rem;
      margin-top: 5%;
    }
    .download_image {
      display: flex;
      flex-direction: column;
      img {
        position: relative;
      }
      .chip {
        position: absolute;
        left: -5%;
        top: 12%;
      }
      a {
        text-align: center;
      }
    }
  }
}
</style>
