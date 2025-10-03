<script setup>
import LanguageSwitcher from './LanguageSwitcher.vue'
import { useI18n } from 'vue-i18n'

defineProps({
  msg: {
    type: String,
    required: true
  }
})

const { t } = useI18n()
</script>

<template>
  <header class="l-header" id="header">
    <nav class="nav bd-container">
      <a href="/" class="nav__logo">{{ t('nav.logo') }}</a>

      <div class="nav__menu nav-center" id="nav-menu">
        <ul class="nav__list">
          <li class="nav__item dropdown dropdown-toggle"><a href="#" class="nav__link active-link">{{ t('nav.platform') }}</a>
            <div class="dropdown-content">
              <div class="dropdown-column">
                <h4>{{ t('nav.pages') }}</h4>
                <a href="/About">{{ t('nav.about') }}</a>
                <a href="/Contact">{{ t('nav.contact') }}</a>
                <a href="/privacy-policy">{{ t('nav.privacyPolicy') }}</a>
                <a href="/terms-and-conditions">{{ t('nav.termsConditions') }}</a>
              </div>
            </div>
          </li>
          <li class="nav__item dropdown dropdown-toggle"><a href="#" class="nav__link">{{ t('nav.partners') }}</a>
            <div class="dropdown-content">
              <div class="dropdown-column">
                <h4>{{ t('nav.partnersTitle') }}</h4>
                <a href="/BecomePartner">{{ t('nav.becomePartner') }}</a>
                <a href="/PartnerPrograms">{{ t('nav.partnerPrograms') }}</a>
              </div>
            </div>
          </li>
          <li class="nav__item dropdown dropdown-toggle">
            <a href="#" class="nav__link">{{ t('nav.resources') }}</a>
            <div class="dropdown-content">
              <div class="dropdown-column">
                <h4>{{ t('nav.resourcesTitle') }}</h4>
                <a href="/Blog">{{ t('nav.blog') }}</a>
                <a href="/Events">{{ t('nav.events') }}</a>
                <a href="#">{{ t('nav.demo') }}</a>
                <a href="#">{{ t('nav.products') }}</a>
              </div>
              <div class="dropdown-column">
                <h4>{{ t('nav.community') }}</h4>
                <a href="/community">{{ t('nav.joinCommunity') }}</a>
                <a href="#">{{ t('nav.contribute') }}</a>
                <a href="/Forum">{{ t('nav.forum') }}</a>
                <a href="#">{{ t('nav.chat') }}</a>
              </div>
            </div>
          </li>
          <li class="nav__item"><a href="#" class="nav__link position-relative"><i class="bi bi-bell-fill"></i>
            <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-success">
              <!-- number of notifications goes here -->
              <span class="visually-hidden">unread messages</span>
            </span>
            Notifications
          </a>
        </li>
        <!--li class="nav__item"><a href="/Login" class="nav__link">{{ t('nav.login') }}</a></li-->
        <li class="nav__item nav_right dropdown dropdown-toggle"><a href="/Account" class="nav__link">Account</a>
          <div class="dropdown-content">
            <div class="dropdown-column">
              <h4>ACCOUNT</h4>
              <a href="/Account">My Profile</a>
              <a href="#">Chat An Expert</a>
              <a href="#">Settings</a>
              <a href="#">Logout</a>
            </div>
          </div>
        </li>
        <!--li class="nav__item"><LanguageSwitcher /></li-->
        <li><i class='bx bx-moon change-theme' id="theme-button"></i></li>
      </ul>
    </div>

    <div class="nav__toggle" id="nav-toggle">
      <i class='bx bx-menu'></i>
    </div>
    </nav>
  </header>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .greetings h1,
  .greetings h3 {
    text-align: left;
  }
}
</style>
