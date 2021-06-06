<template>
  <div class="page-home">
    <div class="intro">
      <div class="row">
        <div class="col-lg-6 col-12 d-flex align-items-start justify-content-center flex-column">
          <h1>
            {{ $t('page.1.intro.title.1') }}
            <br>
            <strong>{{ $t('page.1.intro.title.2') }}</strong>
          </h1>
          <p class="pt-3">
            {{ $t('page.1.intro.subtitle') }}
          </p>
        </div>
      </div>
    </div>
    <div class="road">
      <div class="road-card road-card-1 road-card-left">
        <img src="~/assets/img/home/road-card/1-mob.png" alt="Road card image">
        <div class="number">#1</div>
        <div class="road-card-content">
          <h2>{{ $t('page.1.card.1.title') }}</h2>
          <p>
            {{ $t('page.1.card.1.body') }}
          </p>
          <button @click="$router.push(localePath('jelgava'))" class="btn btn-success mt-5">
            {{ $t('more') }}
          </button>
        </div>
      </div>
      <div class="road-card road-card-2 road-card-right">
        <img src="~/assets/img/home/road-card/2-mob.png" alt="Road card image">
        <div class="number">#2</div>
        <div class="road-card-content">
          <h2>{{ $t('page.1.card.2.title') }}</h2>
          <p>
            {{ $t('page.1.card.2.body') }}
          </p>
          <button @click="$router.push(localePath('brauciens-lidz-rigai'))" class="btn btn-success mt-5">
            {{ $t('more') }}
          </button>
        </div>
      </div>
      <div class="road-card road-card-3 road-card-left">
        <img src="~/assets/img/home/road-card/3-mob.png" alt="Road card image">
        <div class="number">#3</div>
        <div class="road-card-content">
          <h2>{{ $t('page.1.card.3.title') }}</h2>
          <p>
            {{ $t('page.1.card.3.body') }}
          </p>
          <button @click="$router.push(localePath('tornakalns'))" class="btn btn-success mt-5">
            {{ $t('more') }}
          </button>
        </div>
      </div>
      <div class="road-card road-card-4 road-card-right">
        <img src="~/assets/img/home/road-card/4-mob.png" alt="Road card image">
        <div class="number">#4</div>
        <div class="road-card-content">
          <h2>{{ $t('page.1.card.4.title') }}</h2>
          <p>
            {{ $t('page.1.card.4.body') }}
          </p>
          <button @click="$router.push(localePath('biroja'))" class="btn btn-success mt-5">
            {{ $t('more') }}
          </button>
        </div>
      </div>
      <div class="road-card road-card-5 road-card-left">
        <img src="~/assets/img/home/road-card/5-mob.png" alt="Road card image">
        <div class="number">#5</div>
        <div class="road-card-content">
          <h2>{{ $t('page.1.card.5.title') }}</h2>
          <p>
            {{ $t('page.1.card.5.body') }}
          </p>
          <button @click="$router.push(localePath('latvijas-universitate'))" class="btn btn-success mt-5">
            {{ $t('more') }}
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
  .page-home {
    @media (max-width: 992px) {
      background-position-y: 10vh;
      background-image: url('~assets/img/background.png');
      background-repeat: repeat-y;
      background-size: cover;
    }
  }
  .intro {
    background-image: url('~assets/img/home/intro2.png');
    background-repeat: no-repeat;
    background-position: top right;
    background-size: contain;
    height: 70vh;
    position: relative;
    padding: 0 5vw;
    .row {
      height: 100%;
      @media (max-width: 992px) {
        padding-top: 70%;
      }
    }
    h1 {
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
  }
  .road {
    @media (min-width: 992px) {
      background-image: url('~assets/img/background.png');
      background-repeat: repeat-y;
      background-size: cover;
      padding-top: 10vh;
    }
  }
  .road-card {
    position: relative;
    margin: 10vh 0;
    background-repeat: no-repeat;
    background-size: contain;
    @media (max-width: 992px) {
      background: none!important;
    }
    @media (min-width: 992px) {
      width: 80vw;
      box-shadow: 0 0  50px grey;
      //padding: 5vw;
      background-color: white;
    }
    img {
      display: none;
      @media (max-width: 992px) {
        display: block;
        width: 70%;
        margin-left: auto;
      }
    }
    &-content {
      //min-height: 50vh;
      width: 60%;
      position: relative;
      padding: 5vh 0;
      h2 {
        font-size: 64px;
      }
      p {
        font-size: 22px;
        font-weight: 300;
      }
      @media (max-width: 992px) {
        padding: 0 5vw;
        width: unset;
      }
    }
    .number {
      font-weight: bold;
      top: 0;
      left: 0;
      color: #d8d8d8;
      font-family: 'Poppins', sans-serif;
      font-size: 100px;
      line-height: 100px;
      z-index: 0;
      padding: 0 5vw;
      @media (min-width: 992px) {
        padding: 0;
        color: #E1E6F3;
        position: absolute;
        font-size: 288px;
        line-height: 288px;
      }
    }
    @media (min-width: 992px) {
      &-left {
        margin-right: auto;
        background-position: top right;
        .road-card-content {
          margin-left: 5vh;
          margin-right: auto;
        }
      }
      &-right {
        .road-card-content {
          margin-right: 5vh;
          margin-left: auto;
        }
        margin-left: auto;
        background-position: top left;
        .number {
          left: unset;
          right: 0;
        }

        .road-card-content {
          text-align: right;
        }
      }
    }
  }
  .road-card-1 {
    background-image: url('~assets/img/home/road-card/1.png');
  }
  .road-card-2 {
    background-image: url('~assets/img/home/road-card/2.png');
  }
  .road-card-3 {
    background-image: url('~assets/img/home/road-card/3.png');
  }
  .road-card-4 {
    background-image: url('~assets/img/home/road-card/4.png');
  }
  .road-card-5 {
    background-image: url('~assets/img/home/road-card/5.png');
  }
</style>
