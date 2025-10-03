<script setup>
import { useI18n } from 'vue-i18n'

const { t } = useI18n()
</script>

<template>

    <main class="l-main">
        <!--========== HERO SECTION ==========-->
        <section class="services section bd-container" id="services">
            <div style="text-align: center;">
                <div class="home__data">
                    <h1 class="home__title">{{ t('community.title') }}</h1>
                    <p class="home__description">{{ t('community.subtitle') }}</p>
                </div>
            </div>
        </section>

        <!---------- Community Body ----------->
        <section class="section1 bd-container">
            <!-- Community Welcome -->
            <div class="feature-bg">
                <div class="container">
                    <div class="home__container bd-container bd-grid">
                        <div class="home__data">
                            <h2 class="section-title">{{ t('community.welcomeTitle') }}</h2>
                            <p class="about__description">{{ t('community.welcomeDesc') }}</p>
                            
                            <div class="row" style="margin-top: 3rem;">
                                <div class="col-lg-6 col-md-6 mb-4 mb-md-5">
                                    <div class="list-box d-flex">
                                        <div class="content">
                                            <h3>{{ t('community.connectTitle') }}</h3>
                                            <p>{{ t('community.connectDesc') }}</p>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-lg-6 col-md-6 mb-5 mb-md-5">
                                    <div class="list-box d-flex">
                                        <div class="content">
                                            <h3>{{ t('community.supportTitle') }}</h3>
                                            <p>{{ t('community.supportDesc') }}</p>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-lg-6 col-md-6 mb-5 mb-md-5">
                                    <div class="list-box d-flex">
                                        <div class="content">
                                            <h3>{{ t('community.shareTitle') }}</h3>
                                            <p>{{ t('community.shareDesc') }}</p>
                                        </div>
                                    </div>
                                </div>
                                <div class="col-lg-6 col-md-6 mb-5 mb-md-5">
                                    <div class="list-box d-flex">
                                        <div class="content">
                                            <h3>{{ t('community.growTitle') }}</h3>
                                            <p>{{ t('community.growDesc') }}</p>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    
                        <img src="../assets/img/home.jpg" alt="" class="home__img">
                    </div>
                </div>
            </div>

            <!-- Discord CTA Section -->
            <div class="mt-150 mb-150">
                <div class="container">
                    <div class="discord-cta" style="text-align: center; background: linear-gradient(135deg, var(--first-color-lighten) 0%, var(--first-color-alt) 100%); padding: 3rem; border-radius: 1rem; box-shadow: 0 4px 20px rgba(0,0,0,0.1);">
                        <div style="max-width: 700px; margin: 0 auto;">
                            <h2 style="font-size: 2.5rem; margin-bottom: 1rem; color: var(--title-color);">{{ t('community.discordTitle') }}</h2>
                            <p style="font-size: 1.2rem; margin-bottom: 2rem; color: var(--text-color);">{{ t('community.discordDesc') }}</p>
                            
                            <a href="https://discord.gg/RxG3NyQftq" 
                               target="_blank" 
                               rel="noopener noreferrer"
                               class="button"
                               style="display: inline-flex; align-items: center; gap: 0.5rem; font-size: 1.2rem; padding: 1rem 2rem;">
                                <svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor">
                                    <path d="M20.317 4.37a19.791 19.791 0 0 0-4.885-1.515a.074.074 0 0 0-.079.037c-.21.375-.444.864-.608 1.25a18.27 18.27 0 0 0-5.487 0a12.64 12.64 0 0 0-.617-1.25a.077.077 0 0 0-.079-.037A19.736 19.736 0 0 0 3.677 4.37a.07.07 0 0 0-.032.027C.533 9.046-.32 13.58.099 18.057a.082.082 0 0 0 .031.057a19.9 19.9 0 0 0 5.993 3.03a.078.078 0 0 0 .084-.028a14.09 14.09 0 0 0 1.226-1.994a.076.076 0 0 0-.041-.106a13.107 13.107 0 0 1-1.872-.892a.077.077 0 0 1-.008-.128a10.2 10.2 0 0 0 .372-.292a.074.074 0 0 1 .077-.01c3.928 1.793 8.18 1.793 12.062 0a.074.074 0 0 1 .078.01c.12.098.246.198.373.292a.077.077 0 0 1-.006.127a12.299 12.299 0 0 1-1.873.892a.077.077 0 0 0-.041.107c.36.698.772 1.362 1.225 1.993a.076.076 0 0 0 .084.028a19.839 19.839 0 0 0 6.002-3.03a.077.077 0 0 0 .032-.054c.5-5.177-.838-9.674-3.549-13.66a.061.061 0 0 0-.031-.03zM8.02 15.33c-1.183 0-2.157-1.085-2.157-2.419c0-1.333.956-2.419 2.157-2.419c1.21 0 2.176 1.096 2.157 2.42c0 1.333-.956 2.418-2.157 2.418zm7.975 0c-1.183 0-2.157-1.085-2.157-2.419c0-1.333.955-2.419 2.157-2.419c1.21 0 2.176 1.096 2.157 2.42c0 1.333-.946 2.418-2.157 2.418z"/>
                                </svg>
                                {{ t('community.joinDiscord') }}
                            </a>
                            
                            <p style="margin-top: 1.5rem; font-size: 0.9rem; color: var(--text-color); opacity: 0.8;">
                                {{ t('community.discordNote') }}
                            </p>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Additional Info Section -->
            <div class="container" style="margin-bottom: 3rem;">
                <div style="text-align: center; max-width: 800px; margin: 0 auto;">
                    <h3 style="margin-bottom: 1.5rem;">{{ t('community.whyJoinTitle') }}</h3>
                    <p style="line-height: 1.8; color: var(--text-color);">
                        {{ t('community.whyJoinDesc') }}
                    </p>
                </div>
            </div>
            <!-- Community Body End -->
        </section>
        <!---------- Community Body End ----------->

    </main>

</template>

<style scoped>
.discord-cta {
    transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.discord-cta:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 30px rgba(0,0,0,0.15);
}

.button {
    transition: all 0.3s ease;
}

.button:hover {
    transform: scale(1.05);
    box-shadow: 0 4px 15px rgba(0,0,0,0.2);
}
</style>
