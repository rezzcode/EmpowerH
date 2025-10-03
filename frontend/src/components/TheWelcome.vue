<script setup>
import { useI18n } from 'vue-i18n'

const { t } = useI18n()
</script>

<template>
  <main class="l-main">

  <!---- Hero Section ----->
  <section class="hero-section">
    <div class="container">
      <div class="row align-items-center min-vh-75">
        <div class="col-lg-6 text-center text-lg-start order-lg-1 hero-content">
          <div class="hero-badge mb-3">
            <span class="badge-dot"></span>
            {{ t('home.badge') }}
          </div>
          <h1 class="hero-title mb-4">
            {{ t('home.title') }} <span class="gradient-text">{{ t('nav.logo') }}</span>
          </h1>
          <p class="hero-subtitle mb-4">
            {{ t('home.subtitle') }}
          </p>
          <div class="hero-actions">
            <a class="btn btn-primary btn-lg rounded-pill px-4 me-3 btn-hover-lift" href="/signup" role="button">
              <i class="bi bi-arrow-right-circle me-2"></i>{{ t('home.getStarted') }}
            </a>
            <a class="btn btn-outline-primary btn-lg rounded-pill px-4 btn-hover-lift" href="/about" role="button">
              {{ t('home.learnMore') }}
            </a>
          </div>
          <div class="hero-stats mt-5">
            <div class="stat-item">
              <div class="stat-number">10K+</div>
              <div class="stat-label">{{ t('home.stats.users') }}</div>
            </div>
            <div class="stat-item">
              <div class="stat-number">500+</div>
              <div class="stat-label">{{ t('home.stats.stories') }}</div>
            </div>
            <div class="stat-item">
              <div class="stat-number">24/7</div>
              <div class="stat-label">{{ t('home.stats.support') }}</div>
            </div>
          </div>
        </div>
        <div class="col-lg-6 order-lg-2 text-center hero-image-container">
          <div class="hero-image-wrapper">
            <img class="img-fluid hero-image" src="../assets/img/illustrations/hero-header.png" alt="EmpowerH Community" />
            <div class="hero-decoration decoration-1"></div>
            <div class="hero-decoration decoration-2"></div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!---- Mission Section ----->
  <section class="mission-section py-6">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-6 mb-4 mb-lg-0">
          <div class="mission-image-wrapper">
            <img class="img-fluid rounded-4 shadow-lg" src="../assets/img/illustrations/about.png" alt="Our Mission" />
          </div>
        </div>
        <div class="col-lg-6 ps-lg-5">
          <div class="mission-content">
            <span class="section-badge mb-3">Our Mission</span>
            <h2 class="section-title mb-4">Why <span class="gradient-text">EmpowerH</span>?</h2>
            <p class="section-description mb-4">
              EmpowerH is a comprehensive platform dedicated to empowering everyone and providing a safe, inclusive space 
              for connection, support, and growth. Our mission is to foster solidarity and break the silence surrounding 
              gender-based violence and discrimination.
            </p>
            <ul class="mission-features">
              <li class="feature-item">
                <i class="bi bi-check-circle-fill text-success me-2"></i>
                Safe space for sharing stories and experiences
              </li>
              <li class="feature-item">
                <i class="bi bi-check-circle-fill text-success me-2"></i>
                Comprehensive health and wellness resources
              </li>
              <li class="feature-item">
                <i class="bi bi-check-circle-fill text-success me-2"></i>
                Professional support and guidance available
              </li>
              <li class="feature-item">
                <i class="bi bi-check-circle-fill text-success me-2"></i>
                Community-driven empowerment initiatives
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>


  <!---- Features Section ----->
  <section class="features-section py-6">
    <div class="container">
      <div class="text-center mb-5">
        <span class="section-badge mb-3">What We Offer</span>
        <h2 class="section-title mb-3">Powerful Features for <span class="gradient-text">Your Journey</span></h2>
        <p class="section-description">Comprehensive tools and resources designed to support and empower you</p>
      </div>
      
      <div class="row g-4">
        <div class="col-md-6 col-lg-3">
          <div class="feature-card h-100">
            <div class="feature-icon mb-3">
              <img src="../assets/img/illustrations/feature-search.png" alt="Health Track" />
            </div>
            <h4 class="feature-title mb-3">Health Track Platform</h4>
            <p class="feature-description mb-3">
              Comprehensive health tracking to help you manage your physical and mental well-being with ease.
            </p>
            <a class="feature-link" href="/wellness">
              Explore <i class="bi bi-arrow-right ms-1"></i>
            </a>
          </div>
        </div>
        
        <div class="col-md-6 col-lg-3">
          <div class="feature-card h-100">
            <div class="feature-icon mb-3">
              <img src="../assets/img/illustrations/feature-hour.png" alt="Resource Hub" />
            </div>
            <h4 class="feature-title mb-3">Resource Hub</h4>
            <p class="feature-description mb-3">
              Access to helplines, legal aid services, and educational resources all in one place.
            </p>
            <a class="feature-link" href="/sexual-awareness">
              Explore <i class="bi bi-arrow-right ms-1"></i>
            </a>
          </div>
        </div>
        
        <div class="col-md-6 col-lg-3">
          <div class="feature-card h-100">
            <div class="feature-icon mb-3">
              <img src="../assets/img/illustrations/feature-print.png" alt="Story Sharing" />
            </div>
            <h4 class="feature-title mb-3">Story Sharing</h4>
            <p class="feature-description mb-3">
              Share your experiences and connect with others in a safe, supportive environment.
            </p>
            <a class="feature-link" href="/blog">
              Explore <i class="bi bi-arrow-right ms-1"></i>
            </a>
          </div>
        </div>
        
        <div class="col-md-6 col-lg-3">
          <div class="feature-card h-100">
            <div class="feature-icon mb-3">
              <img src="../assets/img/illustrations/feature-security.png" alt="Safe Environment" />
            </div>
            <h4 class="feature-title mb-3">Safe & Inclusive</h4>
            <p class="feature-description mb-3">
              A secure, non-judgmental space where everyone feels valued, respected, and supported.
            </p>
            <a class="feature-link" href="/privacy-policy">
              Explore <i class="bi bi-arrow-right ms-1"></i>
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!---- Testimonials Section ----->
  <section class="testimonial-section py-6">
    <div class="container">
      <div class="text-center mb-5">
        <span class="section-badge mb-3">Community Voices</span>
        <h2 class="section-title mb-3">What Our <span class="gradient-text">Members Say</span></h2>
        <p class="section-description">Real stories from real people in our community</p>
      </div>
      
      <div id="carouselTestimonials" class="carousel slide" data-bs-ride="carousel">
        <div class="carousel-inner">
          <div class="carousel-item active">
            <div class="row justify-content-center">
              <div class="col-lg-8">
                <div class="testimonial-card">
                  <div class="testimonial-stars mb-3">
                    <i class="bi bi-star-fill"></i>
                    <i class="bi bi-star-fill"></i>
                    <i class="bi bi-star-fill"></i>
                    <i class="bi bi-star-fill"></i>
                    <i class="bi bi-star-fill"></i>
                  </div>
                  <p class="testimonial-text mb-4">
                    "EmpowerH has been a transformative experience for me. The community support and resources 
                    have helped me find my voice and connect with amazing people who understand my journey."
                  </p>
                  <div class="testimonial-author">
                    <img src="../assets/img/user-image.svg" alt="Sarah M." class="author-avatar">
                    <div class="author-details">
                      <h5 class="author-name mb-0">Sarah M.</h5>
                      <p class="author-role mb-0">Community Member</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          
          <div class="carousel-item">
            <div class="row justify-content-center">
              <div class="col-lg-8">
                <div class="testimonial-card">
                  <div class="testimonial-stars mb-3">
                    <i class="bi bi-star-fill"></i>
                    <i class="bi bi-star-fill"></i>
                    <i class="bi bi-star-fill"></i>
                    <i class="bi bi-star-fill"></i>
                    <i class="bi bi-star-fill"></i>
                  </div>
                  <p class="testimonial-text mb-4">
                    "The health tracking features and resource hub have been incredibly valuable. I finally have 
                    a safe space to prioritize my wellbeing and access the support I need."
                  </p>
                  <div class="testimonial-author">
                    <img src="../assets/img/user-image.svg" alt="Jessica K." class="author-avatar">
                    <div class="author-details">
                      <h5 class="author-name mb-0">Jessica K.</h5>
                      <p class="author-role mb-0">Wellness Advocate</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          
          <div class="carousel-item">
            <div class="row justify-content-center">
              <div class="col-lg-8">
                <div class="testimonial-card">
                  <div class="testimonial-stars mb-3">
                    <i class="bi bi-star-fill"></i>
                    <i class="bi bi-star-fill"></i>
                    <i class="bi bi-star-fill"></i>
                    <i class="bi bi-star-fill"></i>
                    <i class="bi bi-star-fill"></i>
                  </div>
                  <p class="testimonial-text mb-4">
                    "Sharing my story here helped me heal and connect with others who've been through similar 
                    experiences. This platform is truly empowering and life-changing."
                  </p>
                  <div class="testimonial-author">
                    <img src="../assets/img/user-image.svg" alt="Maria L." class="author-avatar">
                    <div class="author-details">
                      <h5 class="author-name mb-0">Maria L.</h5>
                      <p class="author-role mb-0">Survivor & Advocate</p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselTestimonials" data-bs-slide="prev">
          <span class="carousel-control-icon"><i class="bi bi-chevron-left"></i></span>
          <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselTestimonials" data-bs-slide="next">
          <span class="carousel-control-icon"><i class="bi bi-chevron-right"></i></span>
          <span class="visually-hidden">Next</span>
        </button>
      </div>
    </div>
  </section>

  <!---- CTA Section ----->
  <section class="cta-section py-6">
    <div class="container">
      <div class="cta-card text-center">
        <h2 class="cta-title mb-4">Ready to Join Our Community?</h2>
        <p class="cta-description mb-4">
          Start your journey towards empowerment, healing, and connection today.
        </p>
        <div class="cta-actions">
          <a class="btn btn-light btn-lg rounded-pill px-5 me-3 btn-hover-lift" href="/signup" role="button">
            Get Started Now
          </a>
          <a class="btn btn-outline-light btn-lg rounded-pill px-5 btn-hover-lift" href="/contact" role="button">
            Contact Us
          </a>
        </div>
      </div>
    </div>
  </section>
  </main>
</template>

<style scoped>
/* Hero Section */
.hero-section {
  padding: 80px 0 60px;
  position: relative;
  overflow: hidden;
}

.min-vh-75 {
  min-height: 75vh;
}

.hero-badge {
  display: inline-flex;
  align-items: center;
  padding: 8px 20px;
  background: linear-gradient(135deg, rgba(255, 107, 0, 0.1), rgba(138, 43, 226, 0.1));
  border-radius: 50px;
  font-size: 0.9rem;
  font-weight: 500;
  color: var(--first-color);
}

.badge-dot {
  width: 8px;
  height: 8px;
  background: var(--first-color);
  border-radius: 50%;
  margin-right: 10px;
  animation: pulse 2s infinite;
}

@keyframes pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.5; }
}

.hero-title {
  font-size: clamp(2.5rem, 5vw, 4rem);
  font-weight: 800;
  line-height: 1.2;
  color: var(--title-color);
}

.gradient-text {
  background: linear-gradient(135deg, #ff6b00, #8a2be2);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.hero-subtitle {
  font-size: 1.125rem;
  line-height: 1.8;
  color: var(--text-color);
  opacity: 0.9;
}

.hero-actions {
  display: flex;
  gap: 15px;
  flex-wrap: wrap;
}

.btn-hover-lift {
  transition: all 0.3s ease;
}

.btn-hover-lift:hover {
  transform: translateY(-3px);
  box-shadow: 0 10px 25px rgba(0, 0, 0, 0.15);
}

.hero-stats {
  display: flex;
  gap: 40px;
  flex-wrap: wrap;
}

.stat-item {
  text-align: left;
}

.stat-number {
  font-size: 2rem;
  font-weight: 700;
  color: var(--first-color);
  line-height: 1;
}

.stat-label {
  font-size: 0.875rem;
  color: var(--text-color);
  opacity: 0.8;
  margin-top: 5px;
}

.hero-image-wrapper {
  position: relative;
  z-index: 1;
}

.hero-image {
  animation: float 6s ease-in-out infinite;
}

@keyframes float {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-20px); }
}

.hero-decoration {
  position: absolute;
  border-radius: 50%;
  background: linear-gradient(135deg, rgba(255, 107, 0, 0.1), rgba(138, 43, 226, 0.1));
  z-index: -1;
}

.decoration-1 {
  width: 300px;
  height: 300px;
  top: -50px;
  right: -50px;
}

.decoration-2 {
  width: 200px;
  height: 200px;
  bottom: -50px;
  left: -30px;
}

/* Mission Section */
.mission-section {
  background: linear-gradient(180deg, transparent, rgba(255, 107, 0, 0.03));
  padding: 80px 0;
}

.section-badge {
  display: inline-block;
  padding: 6px 16px;
  background: rgba(255, 107, 0, 0.1);
  color: var(--first-color);
  border-radius: 20px;
  font-size: 0.875rem;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 0.5px;
}

.section-title {
  font-size: clamp(2rem, 4vw, 3rem);
  font-weight: 700;
  color: var(--title-color);
}

.section-description {
  font-size: 1.125rem;
  color: var(--text-color);
  opacity: 0.9;
  max-width: 600px;
  margin: 0 auto;
}

.mission-image-wrapper img {
  transition: transform 0.3s ease;
}

.mission-image-wrapper:hover img {
  transform: scale(1.02);
}

.mission-features {
  list-style: none;
  padding: 0;
}

.feature-item {
  padding: 12px 0;
  font-size: 1.05rem;
  color: var(--text-color);
  display: flex;
  align-items: center;
}

/* Features Section */
.features-section {
  background: var(--body-color);
  padding: 80px 0;
}

.feature-card {
  background: var(--container-color);
  border-radius: 20px;
  padding: 30px;
  transition: all 0.3s ease;
  border: 1px solid rgba(255, 107, 0, 0.1);
}

.feature-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 20px 40px rgba(0, 0, 0, 0.1);
  border-color: var(--first-color);
}

.feature-icon {
  width: 80px;
  height: 80px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: linear-gradient(135deg, rgba(255, 107, 0, 0.1), rgba(138, 43, 226, 0.1));
  border-radius: 15px;
  margin: 0 auto;
}

.feature-icon img {
  width: 50px;
  height: 50px;
  object-fit: contain;
}

.feature-title {
  font-size: 1.25rem;
  font-weight: 600;
  color: var(--title-color);
}

.feature-description {
  font-size: 0.95rem;
  color: var(--text-color);
  opacity: 0.85;
  line-height: 1.6;
}

.feature-link {
  color: var(--first-color);
  text-decoration: none;
  font-weight: 600;
  transition: all 0.3s ease;
  display: inline-flex;
  align-items: center;
}

.feature-link:hover {
  gap: 8px;
  color: var(--first-color-alt);
}

/* Testimonials Section */
.testimonial-section {
  background: linear-gradient(180deg, rgba(255, 107, 0, 0.03), transparent);
  padding: 80px 0;
}

.testimonial-card {
  background: var(--container-color);
  border-radius: 20px;
  padding: 40px;
  text-align: center;
  border: 1px solid rgba(255, 107, 0, 0.1);
}

.testimonial-stars {
  color: #ffc107;
  font-size: 1.25rem;
}

.testimonial-text {
  font-size: 1.125rem;
  line-height: 1.8;
  color: var(--text-color);
  font-style: italic;
}

.testimonial-author {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 15px;
}

.author-avatar {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  border: 3px solid var(--first-color);
}

.author-details {
  text-align: left;
}

.author-name {
  font-size: 1.125rem;
  font-weight: 600;
  color: var(--title-color);
}

.author-role {
  font-size: 0.875rem;
  color: var(--text-color);
  opacity: 0.7;
}

.carousel-control-icon {
  width: 50px;
  height: 50px;
  background: var(--container-color);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--first-color);
  font-size: 1.5rem;
  border: 1px solid rgba(255, 107, 0, 0.2);
  transition: all 0.3s ease;
}

.carousel-control-icon:hover {
  background: var(--first-color);
  color: white;
}

.carousel-control-prev,
.carousel-control-next {
  width: auto;
  opacity: 1;
}

/* CTA Section */
.cta-section {
  padding: 80px 0;
}

.cta-card {
  background: linear-gradient(135deg, #ff6b00, #8a2be2);
  border-radius: 30px;
  padding: 60px 40px;
  color: white;
}

.cta-title {
  font-size: clamp(2rem, 4vw, 3rem);
  font-weight: 700;
  color: white;
}

.cta-description {
  font-size: 1.25rem;
  color: rgba(255, 255, 255, 0.9);
  max-width: 600px;
  margin: 0 auto;
}

.cta-actions {
  display: flex;
  gap: 15px;
  justify-content: center;
  flex-wrap: wrap;
}

/* Responsive Adjustments */
@media (max-width: 768px) {
  .hero-section {
    padding: 60px 0 40px;
  }
  
  .hero-stats {
    gap: 20px;
  }
  
  .stat-number {
    font-size: 1.5rem;
  }
  
  .feature-card {
    padding: 25px;
  }
  
  .testimonial-card {
    padding: 30px 20px;
  }
  
  .cta-card {
    padding: 40px 20px;
  }
  
  .hero-actions,
  .cta-actions {
    flex-direction: column;
  }
  
  .hero-actions .btn,
  .cta-actions .btn {
    width: 100%;
  }
}
</style>
