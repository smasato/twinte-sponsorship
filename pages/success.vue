<template>
  <section class="section">
    <h1 class="title">
      ありがとうございました!
    </h1>
    <p>
      寄付金の受付が完了しました。
      <br>
      <nuxt-link to="/mypage">
        マイページ
      </nuxt-link>からユーザー情報の編集や寄付の履歴が確認できます。
    </p>
    <p id="share">
      <a
        :data-text="makeText()"
        href="https://twitter.com/share?ref_src=twsrc%5Etfw"
        class="twitter-share-button"
        data-size="large"
        data-url="https://sponsorship.twinte.net"
        data-via="te_twin"
        data-hashtags="Twinte"
        data-related="te_twin"
        data-show-count="false"
      >Tweet</a><script async src="https://platform.twitter.com/widgets.js" charset="utf-8" />
    </p>
  </section>
</template>

<script>
export default {
  computed: {

  },
  methods: {
    makeText () {
      return 'Twin:teに寄付しました！'
    }
  }
}
</script>

<style lang="scss" scoped>
#share{
  margin-top: 1rem;
}
.kind{
  font-style: normal;
  font-weight: bold;
}
.price{
  font-style: normal;
  font-weight: bold;
  font-size: 50px;
  line-height: 72px;
}
</style>
