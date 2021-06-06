<template>
  <b-navbar toggleable type="dark" variant="dark">
    <b-navbar-brand to="/">
      <img src="~/assets/img/logo.png" alt="NT logo">
    </b-navbar-brand>

    <b-navbar-toggle target="sidebar-backdrop">
      <img src="~/assets/img/burger.svg" alt="Burger">
    </b-navbar-toggle>
    <b-sidebar
      id="sidebar-backdrop"
      backdrop-variant="dark"
      backdrop
      shadow
    >
      <template #default="{ hide }">
        <div class="px-3 py-2">
          <nav class="mb-3">
            <b-nav vertical>
              <b-nav-item :to="switchLocalePath('lv')" @click="hide">Latvian</b-nav-item>
              <b-nav-item :to="switchLocalePath('en')" @click="hide">English</b-nav-item>
              <hr>
              <b-nav-item active :to="localePath('index')" @click="hide">{{ $t('pages.0') }}</b-nav-item>
              <b-nav-item :to="localePath('jelgava')" @click="hide">{{ $t('pages.1') }}</b-nav-item>
              <b-nav-item :to="localePath('brauciens-lidz-rigai')" @click="hide">{{ $t('pages.2') }}</b-nav-item>
              <b-nav-item :to="localePath('tornakalns')" @click="hide">{{ $t('pages.3') }}</b-nav-item>
              <b-nav-item :to="localePath('biroja')" @click="hide">{{ $t('pages.4') }}</b-nav-item>
              <b-nav-item :to="localePath('latvijas-universitate')" @click="hide">{{ $t('pages.5') }}</b-nav-item>
              <b-nav-item :to="localePath('skersli-lidz-universitatei')" @click="hide">{{ $t('pages.6') }}</b-nav-item>
              <b-nav-item :to="localePath('par-mani')" @click="hide">{{ $t('pages.7') }}</b-nav-item>
            </b-nav>
          </nav>
        </div>
      </template>
    </b-sidebar>
  </b-navbar>
</template>

<style lang="scss" scoped>
.navbar-dark .navbar-toggler {
  border: none;
}
.navbar-dark {
  padding-left: 5vw;
  padding-right: 5vw;
}
</style>
