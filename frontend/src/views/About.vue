<script setup>
import { useI18n } from 'vue-i18n'

const { t } = useI18n()
</script>

<template>

    <main class="l-main">
        <!--========== HOME ==========-->
        <section class="services section bd-container" id="services">
            <div style="text-align: center;">
                <div class="home__data">
                    <h1 class="home__title">{{ t('about.title') }}</h1>
                </div>
            </div>
        </section>

        <!---------- About us Body ----------->
        <section class="section1 bd-container">
            <!-- About Us -->
            <div class="feature-bg">
                <div class="container">
                    <div class="home__container bd-container bd-grid">
                        <div class="home__data">
                            <div class="row">
                                <div class="col-lg-6 col-md-6 mb-4 mb-md-5">
                                    <div class="list-box d-flex">
                                        <div class="content">
                                            <h3>{{ t('about.privacySafety') }}</h3>
                                            <p>{{ t('about.privacySafetyDesc') }}</p>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-lg-6 col-md-6 mb-5 mb-md-5">
                                    <div class="list-box d-flex">
                                        <div class="content">
                                            <h3>{{ t('about.safeCommunity') }}</h3>
                                            <p>{{ t('about.safeCommunityDesc') }}</p>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-lg-6 col-md-6 mb-5 mb-md-5">
                                    <div class="list-box d-flex">
                                        <div class="content">
                                            <h3>{{ t('about.empowerEveryone') }}</h3>
                                            <p>{{ t('about.empowerEveryoneDesc') }}</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    
                        <img src="../assets/img/home.jpg" alt="" class="home__img">
                    </div>
                </div>
            </div>

            <div class="mt-150">
                <div class="container">
                    <h3 style="text-align:center">{{ t('about.moreAbout') }}</h3>
                    <br>
                    <p>
                    {{ t('about.intro') }}<br><br>

                    <strong>{{ t('about.mission') }}</strong><br>
                    {{ t('about.missionDesc') }}<br><br>

                    <strong>{{ t('about.whatWeOffer') }}</strong><br>
                    • {{ t('about.offer1') }}<br>
                    • {{ t('about.offer2') }}<br>
                    • {{ t('about.offer3') }}<br>
                    • {{ t('about.offer4') }}<br>
                    • {{ t('about.offer5') }}<br><br>

                    <strong>{{ t('about.commitment') }}</strong><br>
                    {{ t('about.commitmentDesc') }}<br><br>

                    {{ t('about.joinUs') }}
                    </p>
                </div>
            </div>
            <!-- About us End -->
        </section>
        <!---------- About us Body End ----------->

    </main>

</template>
