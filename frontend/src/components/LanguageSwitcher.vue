<script setup>
import { useI18n } from 'vue-i18n'
import { ref } from 'vue'

const { locale } = useI18n()
const showDropdown = ref(false)

const languages = [
  { code: 'en', name: 'English', flag: '🇬🇧' },
  { code: 'fr', name: 'Français', flag: '🇫🇷' },
  { code: 'sw', name: 'Kiswahili', flag: '🇰🇪' }
]

const currentLanguage = ref(languages.find(lang => lang.code === locale.value) || languages[0])

const changeLanguage = (lang) => {
  locale.value = lang.code
  currentLanguage.value = lang
  localStorage.setItem('locale', lang.code)
  showDropdown.value = false
}

const toggleDropdown = () => {
  showDropdown.value = !showDropdown.value
}
</script>

<template>
  <div class="language-switcher">
    <button @click="toggleDropdown" class="lang-button">
      <span class="flag">{{ currentLanguage.flag }}</span>
      <span class="lang-code">{{ currentLanguage.code.toUpperCase() }}</span>
      <i class="bx bx-chevron-down"></i>
    </button>
    <div v-if="showDropdown" class="lang-dropdown">
      <button 
        v-for="lang in languages" 
        :key="lang.code"
        @click="changeLanguage(lang)"
        class="lang-option"
        :class="{ active: lang.code === locale }"
      >
        <span class="flag">{{ lang.flag }}</span>
        <span class="lang-name">{{ lang.name }}</span>
      </button>
    </div>
  </div>
</template>

<style scoped>
.language-switcher {
  position: relative;
  display: inline-block;
}

.lang-button {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.5rem 0.75rem;
  background: transparent;
  border: 1px solid var(--first-color);
  border-radius: 0.5rem;
  color: var(--text-color);
  cursor: pointer;
  transition: all 0.3s;
  font-size: 0.9rem;
}

.lang-button:hover {
  background: var(--first-color);
  color: white;
}

.flag {
  font-size: 1.2rem;
}

.lang-code {
  font-weight: 600;
  font-size: 0.85rem;
}

.lang-dropdown {
  position: absolute;
  top: 100%;
  right: 0;
  margin-top: 0.5rem;
  background: var(--body-color);
  border: 1px solid var(--first-color);
  border-radius: 0.5rem;
  min-width: 180px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  z-index: 1000;
  overflow: hidden;
}

.lang-option {
  display: flex;
  align-items: center;
  gap: 0.75rem;
  width: 100%;
  padding: 0.75rem 1rem;
  background: transparent;
  border: none;
  color: var(--text-color);
  cursor: pointer;
  transition: all 0.3s;
  text-align: left;
}

.lang-option:hover {
  background: var(--first-color);
  color: white;
}

.lang-option.active {
  background: rgba(255, 107, 0, 0.1);
  font-weight: 600;
}

.lang-name {
  font-size: 0.9rem;
}

@media screen and (max-width: 768px) {
  .lang-button {
    padding: 0.4rem 0.6rem;
    font-size: 0.85rem;
  }
  
  .lang-dropdown {
    min-width: 150px;
  }
}
</style>
