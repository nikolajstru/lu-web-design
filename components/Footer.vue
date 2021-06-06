<template>
  <div class="footer position-relative">
    <div class="container">
      <div class="row text-white">
        <div class="col-md-8 col-12">
          <h3>
            {{ $t('menu') }}
          </h3>
          <div class="row">
            <div class="col-md-6 col-12">
              <ul class="list-unstyled text-small">
                <li class="mb-1">
                  <nuxt-link :to="localePath('index')">{{ $t('pages.0') }}</nuxt-link>
                </li>
                <li class="mb-1">
                  <nuxt-link :to="localePath('jelgava')">{{ $t('pages.1') }}</nuxt-link>
                </li>
                <li class="mb-1">
                  <NuxtLink :to="localePath('brauciens-lidz-rigai')">{{ $t('pages.2') }}</NuxtLink>
                </li>
                <li class="mb-1">
                  <NuxtLink :to="localePath('tornakalns')">{{ $t('pages.3') }}</NuxtLink>
                </li>
              </ul>
            </div>
            <div class="col-md-6 col-12">
              <ul class="list-unstyled text-small">
                <li class="mb-1">
                  <NuxtLink :to="localePath('biroja')">{{ $t('pages.4') }}</NuxtLink>
                </li>
                <li class="mb-1">
                  <NuxtLink :to="localePath('latvijas-universitate')">{{ $t('pages.5') }}</NuxtLink>
                </li>
                <li class="mb-1">
                  <NuxtLink :to="localePath('skersli-lidz-universitatei')">{{ $t('pages.6') }}</NuxtLink>
                </li>
                <li class="mb-1">
                  <NuxtLink :to="localePath('par-mani')">{{ $t('pages.7') }}</NuxtLink>
                </li>
              </ul>
            </div>
          </div>
        </div>
        <div class="col-md-4 col-12">
          <h3>
            {{ $t('contacts') }}
          </h3>
          <div>
            <ul class="list-unstyled text-small">
              <li class="mb-1">Nikolajs Trubačistovs nt18013</li>
              <li class="mb-1">nikolajs.trubacistovs@gmail.com</li>
              <li class="mb-1">+371 28229404</li>
              <li class="mb-1">Jelgava</li>
            </ul>
          </div>
        </div>
      </div>
    </div>
    <div class="text-center text-white py-2">
      Copyright © 2021 Nikolajs Trubačistovs
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .footer {
    background-image: url('~assets/img/footer-blob.png');
    background-repeat: no-repeat;
    background-size: cover;
    .container {
      padding: 20vh 0;
    }
    a, li {
      font-weight: 300;
      text-decoration: none;
      color: #bababa;
    }
    @media (max-width: 768px) {
      background-image: url('~assets/img/footer-blob-mob.png');
      h3, a, li {
        text-align: center;
      }
      .container {
        padding: 10vh 0;
      }
    }
  }
</style>
