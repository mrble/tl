<template>
  <div>
    <header>
      <div class="header-contaienr">
        <div class="header">
          <div>TL_mrble</div>
        </div>
      </div>
    </header>
    <nuxt />
    <footer>
      <div class="footer-contaienr">
        <div class="footer">
          <div>降った〜</div>
        </div>
      </div>
    </footer>
  </div>
</template>
<style lang='scss'>
.header-contaienr {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  background: #fff;
}

.header {
  margin: 0 auto;
  width: 1024px;
  padding: 10px;
  border-bottom: solid 1px #e2e8f0;
}

.footer-contaienr {
  width: 100%;
}

.footer {
  margin: 0 auto;
  width: 1024px;
  padding: 10px;
  border-top: solid 1px #e2e8f0;
}

.body {
  display: flex;
  width: 1024px;
  margin: 30px auto 0;
}

.side {
  width: 30%;
  padding: 0 10px 16px 0;
  border-right: solid 1px #e2e8f0;

  ul {
    position: sticky;
    top: 56px;
    overflow-y: scroll;
    height: auto;
  }

  li {
    font-size: 14px;
    line-height: 1.4;

    &:not(:last-child) {
      margin-bottom: 18px;
    }
  }
}

.main {
  padding: 0 0 10px 10px;
  width: 70%;

  p {
    margin-bottom: 12px;
  }
}

.card {
  padding: 18px 12px;
  margin-bottom: 50px;
  border: solid 1px #e2e8f0;
}

h1 {
  font-size: 24px;
  font-weight: bold;
  margin-bottom: 24px;
}

h2 {
  font-size: 20px;
  font-weight: bold;
  margin-top: 30px;
  margin-bottom: 18px;
  padding-bottom: 8px;
  border-bottom: solid 1px #e2e8f0;
}

h3 {
  display: flex;
  font-size: 18px;
  font-weight: bold;
  margin-top: 28px;
  margin-bottom: 16px;

  &::before {
    content: '';
    display: block;
    flex: 0 0 auto;
    width: 4px;
    margin-right: 10px;
    background: #e2e8f0;
  }
}

h4 {
  font-size: 16px;
  font-weight: bold;
  margin-top: 24px;
  margin-bottom: 12px;
}

pre {
  font-size: 14px !important;
}

img {
  width: 100%;
}

</style>
