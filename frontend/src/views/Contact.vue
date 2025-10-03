<script setup>
import { ref } from 'vue'
import { useI18n } from 'vue-i18n'
import api from '../api'
import qs from 'qs'

const { t } = useI18n()

const form = ref({
  email: '',
  full_name: '',
  subject: '',
  phone_number: '',
  message: ''
})

const submitForm = async () => {
  const formData = qs.stringify(form.value)

  try {
    const response = await api.contactForm(formData, {
      headers: {
        'Content-Type': 'application/x-www-form-urlencoded'
      }
    })
    alert('Form submitted successfully!')
  } catch (error) {
    console.error('Error:', error)
    alert('Error submitting form. Please try again later.')
  }
}
</script>

<template>

    <main class="l-main">
        <!--========== HOME ==========-->
        <section class="services section bd-container" id="services">
            <div style="text-align: center;">
                <div class="home__data">
                    <h1 class="home__title">{{ t('contact.title') }}</h1>
                </div>
            </div>
        </section>

        <!---------- Blog Body ----------->
        <section class="section1 bd-container">
            <!-- contact form -->
            <div class="contact-from-section mt-150 mb-150">
              	<div class="container">
                <div class="row">
                  	<div class="col-lg-8 mb-5 mb-lg-0">
                    <div class="form-title">
                    	<h2>{{ t('contact.haveQuestions') }}</h2>
                    	<br>
                    	<p>{{ t('contact.intro') }}</p>
                    </div>
                    <br>
                    <div id="form_status"></div>
                    <div class="contact-form">
                    	<form @submit.prevent="submitForm" class="row g-3">
                        <div class="col-md-6">
                        	<label for="inputEmail4" class="form-label">{{ t('contact.email') }}</label>
                        	<input type="email" class="form-control" v-model="form.email" required>
                        </div>
                        <div class="col-md-6">
                        	<label for="name" class="form-label">{{ t('contact.fullName') }}</label>
                        	<input type="text" class="form-control" v-model="form.full_name" required>
                        </div>
                        <div class="col-md-6">
                        	<label for="subject" class="form-label">{{ t('contact.subject') }}</label>
                        	<input type="text" class="form-control" v-model="form.subject" required>
                        </div>
                        <div class="col-md-6">
                        	<label for="tel" class="form-label">{{ t('contact.phoneNumber') }}</label>
                        	<input type="tel" class="form-control" v-model="form.phone_number" required>
                        </div>
                        <div class="form-floating">
                    	    <textarea class="form-control" :placeholder="t('contact.message')" rows="10" v-model="form.message" style="height: 200px" required></textarea>
                        </div>
                        <div class="col-12">
                	        <button type="submit" class="btn btn-primary">{{ t('contact.submit') }}</button>
                        </div>
            	        </form>
                    </div>
                  	</div>
                  	<div class="col-lg-4">
                    <div class="contact-form-wrap">
        	            <div class="contact-form-box">
                        <h4><i class="bi bi-map-fill"></i> {{ t('contact.ourAddress') }}</h4>
                        <p style="white-space: pre-line">{{ t('contact.address') }}</p>
    	                </div>
    	                <br>
	                    <div class="contact-form-box">
                        <h4><i class="bi bi-clock"></i> {{ t('contact.activeHours') }}</h4>
                        <p style="white-space: pre-line">{{ t('contact.hours') }}</p>
                        </div>
                        <br>
                    	<div class="contact-form-box">
                        <h4><i class="bi bi-journal-richtext"></i> {{ t('contact.contactInfo') }}</h4>
                        <p>{{ t('contact.phone') }} <br> {{ t('contact.emailAddress') }}</p>
                    	</div>
                    </div>
                  	</div>
                </div>
              	</div>
            </div>
            <!-- end contact form -->
        </section>
        <!---------- Blog Body End ----------->

    </main>

</template>
