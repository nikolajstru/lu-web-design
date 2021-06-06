<template>
  <div class="page-jelgava">
    <div class="intro">
      <div class="right d-flex flex-lg-row flex-column-reverse align-items-center h-100">
        <img src="~/assets/img/latvijas-universitate/1.png" alt="">
        <div class="about">
          <h1>
            {{ $t('page.6.1.title') }}
          </h1>
          <p>
            {{ $t('page.6.1.body') }}
          </p>
        </div>
      </div>
    </div>
    <div class="content">
      <div class="left d-flex flex-lg-row flex-column-reverse align-items-center">
        <img src="~/assets/img/latvijas-universitate/2.png" alt=""/>
        <div class="about">
          <h2>
            {{ $t('page.6.1.title') }}
          </h2>
          <p>
            {{ $t('page.6.1.body') }}
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.page-jelgava {
  @media (max-width: 992px) {
    background-position-y: 10vh;
    background-image: url('~assets/img/background.png');
    background-repeat: repeat-y;
    background-size: cover;
  }
}
.intro {
  padding-top: 10vh;
  margin-bottom: 10vh;
  .about {
    padding: 0 5vw;
  }
  @media (min-width: 992px) {
    height: 70vh;
    padding-top: 0;
    background-image: url('~assets/img/latvijas-universitate/1.png');
    background-repeat: no-repeat;
    background-position: top right;
    background-size: contain;
    img {
      display: none;
    }
    .about {
      width: 40vw;
    }
  }
  h1 {
    font-weight: bold;
    font-size: 60px;
    @media (max-width: 992px) {
      font-size: 40px;
    }
  }
  p {
    font-weight: 300;
    font-size: 24px;
    line-height: 40px;
  }
  img {
    width: 80vw;
    margin-left: auto;
  }
}

.content {
  img {
    width: 40vw;
  }
  .left {
    img {
      margin-right: auto!important;
    }
  }
  .right {
    img {
      margin-left: auto!important;;
    }
  }
  .about {
    padding: 0 5vw;
  }
  h2 {
    font-size: 48px;
    @media (max-width: 992px) {
      font-size: 40px;
    }
  }
  p {
    font-weight: 300;
    font-size: 24px;
    line-height: 40px;
  }
  @media (max-width: 992px) {
    img {
      width: 80vw;
    }
  }
}
</style>
