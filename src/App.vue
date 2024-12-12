<script setup>
import Footer from "@/components/Footer.vue";
import Telegram from "@/components/icons/Telegram.vue";
import LinkedIn from "@/components/icons/LinkedIn.vue";
import X from "@/components/icons/X.vue";
import Gmail from "@/components/icons/Gmail.vue";
</script>

<template>
  <div class="screen">
    <div class="hero">
      <section class="section">
        <div class="about">
          <div class="image-container">
            <img
              src="./assets/avatar.jpg"
              alt=""
              oncontextmenu="return false;"
            />
            <div class="overlay"></div>
          </div>

          <div class="details">
            <h1>👋 Hi there! I'm Tim.</h1>
            <p>
              I design thoughtful and user-friendly interfaces that solve
              problems and create delightful digital experiences. My mission is
              to blend aesthetics, functionality, and precision into every
              project I work on.
            </p>
            <div class="tags">
              <div class="tag">UI/UX</div>
              <div class="tag">Prototyping</div>
              <div class="tag">Wireframing</div>
              <div class="tag">Research</div>
            </div>
          </div>
        </div>
        <div class="contacts">
          <p>Let's connect.</p>
          <div class="socials">
            <a
              class="social"
              href="https://t.me/aimtimtimtim"
              target="_blank"
              rel="noopener noreferrer"
            >
              <Telegram />
            </a>
            <a
              class="social"
              href="https://x.com/aimtimtimtim"
              target="_blank"
              rel="noopener noreferrer"
            >
              <X />
            </a>
            <a
              class="social"
              href="mailto:agayevtim@gmail.com"
              target="_blank"
              rel="noopener noreferrer"
            >
              <Gmail />
            </a>
            <!-- <div class="social"><LinkedIn /></div>
            <div class="social"><Gmail /></div>
            <div class="social"><X /></div> -->
          </div>
        </div>
      </section>
    </div>
    <Footer />
  </div>
</template>

<style scoped>
.screen {
  display: flex;
  flex-direction: column;
  min-height: 100dvh;
}
.hero {
  padding: 0 16px; /* Отступы слева и справа по 16px */
  flex-grow: 1;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.section {
  max-width: 600px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 50px;
  width: 100%;
}

.about {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 20px;
  img {
    max-width: 200px;
  }
}

.image-container {
  position: relative;
}

.overlay {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: rgba(255, 255, 255, 0); /* Прозрачный фон */
}

.details {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 20px;
}

.details span {
  max-width: 40px;
}

.details h1 {
  text-align: center;
  font-size: 40px;
  font-weight: 900;
}

.details p {
  font-size: 16px;
  line-height: 150%;
  text-align: center;
}

.tags {
  display: flex;
  gap: 8px;
}

.tag {
  padding: 6px 10px;
  background-color: #f5ebd6;
  line-height: normal;
  font-size: 14px;
  border-radius: 99px;
}
.contacts {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 16px;
}
.socials {
  display: flex;
  gap: 12px;
}
.social {
  transition: box-shadow 0.3s ease, transform 0.2s ease;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 60px;
  width: 60px;
  background-color: #fff;
  border-radius: 18px;
}
.social:hover {
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
  transform: scale(1.1);
}
.contacts p {
  font-size: 18px;
  font-weight: 700;
}
</style>
