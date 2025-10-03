<script setup>
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
  <!------------ FOOTER -------------->
  <footer class="footer section bd-container">

    <!-- footer -->

    <div class="footer-area">
      <div class="container">
        <div class="row">
          <div class="col-lg-3 col-md-6">
            <div class="footer-box about-widget">
              <h2 class="widget-title">{{ t('footer.whyUs') }}</h2>
              <p>{{ t('footer.whyUsDesc') }}</p>
            </div>
          </div>
          <div class="col-lg-3 col-md-6">
            <div class="footer-box get-in-touch">
              <h2 class="widget-title">{{ t('footer.getInTouch') }}</h2>
              <ul>
                <li>34/8, East Karapul, Rabango, SA.</li>
                <li>support@empowerher.com</li>
                <li>+00 111 222 3333</li>
              </ul>
            </div>
          </div>
          <div class="col-lg-3 col-md-6">
            <div class="footer-box pages">
              <h2 class="widget-title">{{ t('footer.pages') }}</h2>
              <ul>
                <li><a href="/" class="footer__link">{{ t('footer.home') }}</a></li>
                <li><a href="about" class="footer__link">{{ t('footer.about') }}</a></li>
                <li><a href="contact" class="footer__link">{{ t('footer.contact') }}</a></li>
                <li><a href="privacy-policy" class="footer__link">{{ t('footer.privacyPolicy') }}</a></li>
              </ul>
            </div>
          </div>
          <div class="col-lg-3 col-md-6">
            <div class="footer-box subscribe">
              <h2 class="widget-title">{{ t('footer.subscribe') }}</h2>
              <p>{{ t('footer.subscribeDesc') }}</p>
              <br>
              <form action="/home">
                <div class="input-group mb-3">
                  <input type="email" class="form-control" placeholder="Email" aria-label="Recipient's username" aria-describedby="basic-addon2" required>
                  <span class="input-group-text" id="basic-addon2">Subscribe</span>
                  <!--button class="btn btn-outline-secondary" type="submit">
                    <i class="bi bi-send"></i>
                  </button-->
                </div>
              </form>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- end footer -->

    <!-- copyright -->
    <div class="copyright">
      <div class="container">
        <div class="row footer__copy">
          <div class="col-lg-6 col-md-12">
            <p>Copyrights &copy; 2024 - <a href="/">EmpowerH</a>, {{ t('footer.copyright') }}
            </p>
          </div>
          <div class="col-lg-6 text-right col-md-12">
            <div class="social-icons">
              <ul>
                <li><a href="https://facebook.com/empowerHerr" target="_blank"><i class="bx bxl-facebook"></i></a></li>
                <li><a href="https://twitter.com/empowerHerr" target="_blank"><i class="bx bxl-twitter"></i></a></li>
                <li><a href="https://instagram.com/empowerHerr" target="_blank"><i class="bx bxl-instagram"></i></a></li>
                <li><a href="https://linkedin.com/in/empowerHerr" target="_blank"><i class="bx bxl-linkedin"></i></a></li>
                <li><a href="https://dribble.com/empowerHerr" target="_blank"><i class="bx bxl-dribbble"></i></a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- end copyright -->
  </footer>
</template>

<style scoped>

</style>
