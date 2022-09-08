<template>
  <div>
    <div class="main-v" />
    <div class="about-wrapper">
      <div id="about" class="about-wrapper__top">
        About
      </div>
      <div class="profile-wrapper">
        <img src="~/assets/image/about.jpg" class="profile-wrapper__image">
        <div class="profile-wrapper__right">
          <div class="profile-wrapper__right--name">
            KAKERU MIYAICHI
          </div>
          <div class="profile-wrapper__right--text">
            テキストテキストテキストテキストテキストテキストテキスト テキストテキストテキストテキストテキストテキストテキスト テキストテキストテキストテキストテキストテキストテキスト
          </div>
        </div>
      </div>
    </div>
    <div class="bicycle-wrapper">
      <div id="bicycle" class="bicycle-wrapper__top">
        Bicycle
      </div>
      <div class="bicycle-wrapper__container">
        <div class="bicycle-wrapper__card">
          <img src="~/assets/image/bicycle1.jpg">
          <div class="bicycle-wrapper__title">
            タイトルタイトル
          </div>
          <div class="bicycle-wrapper__text">
            テキストテキストテキスト
          </div>
        </div>
        <div class="bicycle-wrapper__card">
          <img src="~/assets/image/bicycle2.jpg">
          <div class="bicycle-wrapper__title">
            タイトルタイトル
          </div>
          <div class="bicycle-wrapper__text">
            テキストテキストテキスト
          </div>
        </div>
        <div class="bicycle-wrapper__card">
          <img src="~/assets/image/bicycle3.jpg">
          <div class="bicycle-wrapper__title">
            タイトルタイトル
          </div>
          <div class="bicycle-wrapper__text">
            テキストテキストテキスト
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style lang="scss" scoped>
img{
  width: 100%;
}

.main-v{
  background-image: url(~/assets/image/mainvisual.jpg);
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  height: 600px;
}

.about-wrapper{
  display: flex;
  flex-direction: column;
  align-items: center;
  &__top{
    text-align: left;
    font: normal normal bold 32px/48px Meiryo;
    letter-spacing: 0px;
    color: #383E45;
    opacity: 1;
    border-bottom: solid 1px #383E45;
    width: 101px;
    margin: 80px 0 70px 0;
  }
}
.profile-wrapper{
  display: flex;
  flex-direction: row;
  align-items: center;
  @media screen and (max-width: 599px) {
    flex-direction: column;
  }
  &__image{
    border-radius: 50%;
    padding: 10px;
    width: 100px;
    height: 100px;
  }
  &__right{
    width: 403px;
    text-align: left;
    font: normal normal normal 14px/21px Meiryo;
    letter-spacing: 0px;
    color: #383E45;
    opacity: 1;
    padding: 0 0 0 30px;
    @media screen and (max-width: 599px) {
      width: auto;
      padding: 0 30px;
    }
    &--name{
      padding: 0 0 10px 0;
      font: normal normal bold 16px/24px Meiryo;
    }
  }
}
.bicycle-wrapper{
  display: flex;
  flex-direction: column;
  align-items: center;
  &__top{
    text-align: left;
    font: normal normal bold 32px/48px Meiryo;
    letter-spacing: 0px;
    color: #383E45;
    opacity: 1;
    border-bottom: solid 1px #383E45;
    margin: 100px 0 60px 0;
  }
  &__container{
    display: flex;
    flex-direction: row;
    @media screen and (max-width: 599px) {
      flex-direction: column;
    }
  }
  &__card{
    padding: 8px;
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: left;
    font: normal normal normal 14px/21px Meiryo;
    letter-spacing: 0px;
    color: #383E45;
    opacity: 1;
    img{
      width: 263px;
      @media screen and (max-width: 599px) {
        width: 100%;
      }
    }
  }
  &__title{
    margin: 10px 0 10px 0;
    font: normal normal bold 16px/24px Meiryo;
  }
}
.copy-right{
  text-align: left;
  font: normal normal normal 10px/15px Meiryo;
  letter-spacing: 0px;
  color: #383E45;
  opacity: 1;
  margin: 110px 0 10px 0;
}
</style>