<template>
  <div class="left">
    <div class="background-image"></div>
    <div class="background-gradient"></div>
    <div class="left-inner">
      <div class="info">
        <h1 class="greeting">Hey, I'm Noah Dave</h1>
        <p class="description">A Web Developer based in Nairobi, KE</p>
        <p class="current-role">Software Engineer @ Fusional Tech</p>
      </div>

      <div class="social-links">
        <!-- X (Twitter) -->
        <a href="https://x.com/Noah02Dave" aria-label="X (formerly Twitter)" target="_blank" rel="noopener">
          <i class="fab fa-x-twitter"></i>
        </a>

        <!-- Instagram -->
        <a href="https://www.instagram.com/t3ch.savvy/" aria-label="Instagram" target="_blank" rel="noopener">
          <i class="fab fa-instagram"></i>
        </a>

        <!-- TikTok -->
        <a href="https://www.tiktok.com/@_noah.dave_" aria-label="TikTok" target="_blank" rel="noopener">
          <i class="fab fa-tiktok"></i>
        </a>

        <!-- LinkedIn -->
        <a href="#" aria-label="LinkedIn" target="_blank" rel="noopener">
          <i class="fab fa-linkedin-in"></i>
        </a>

        <!-- GitHub -->
        <a href="https://github.com/DavisNoah02" aria-label="GitHub" target="_blank" rel="noopener">
          <i class="fab fa-github"></i>
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>
// No JS needed here for static content
</script>

<style scoped>
/* Layout */
.left {
  width: 50vw;
  height: 100vh;
  position: fixed;
  left: 0;
  top: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}

.background-image {
  position: absolute;
  inset: 0;
  background: url('../assets/Profile.png') center center/cover no-repeat;
  z-index: 1;
  filter: brightness(0.7);
}

.background-gradient {
  position: absolute;
  inset: 0;
  background: linear-gradient(135deg, rgba(53, 83, 110, 0.85), rgba(28, 120, 71, 0.7));
  z-index: 2;
}

.left-inner {
  position: relative;
  z-index: 3;
  width: 100%;
  height: 100%;
  padding-top: 240px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

/* Info Section */
.info {
  color: #ffffff;
  text-align: center;
  margin-bottom: 40px;
}

.greeting {
  font-size: 2.5rem;
  font-weight: 600;
  margin-bottom: 20px;
}

.description,
.current-role {
  font-size: 1.2rem;
  font-weight: 300;
  margin-bottom: 10px;
  opacity: 0.95;
}

/* Social Links */
.social-links {
  display: flex;
  gap: 20px;
  justify-content: center;
}

.social-links a {
  color: #ffffff;
  font-size: 1.4rem;
  width: 44px;
  height: 44px;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 12px;
  background-color: rgba(255, 255, 255, 0.05);
  border: 1px solid rgba(255, 255, 255, 0.1);
  transition: all 0.3s ease;
}

.social-links a:hover {
  transform: scale(1.1);
  background-color: rgba(255, 255, 255, 0.1);
  border-color: rgba(255, 255, 255, 0.3);
}

/* Brand Hover Effects */
.social-links a[aria-label='X (formerly Twitter)']:hover {
  color: #000;
  background-color: #fff;
}

.social-links a[aria-label='Instagram']:hover {
  color: #e1306c;
}

.social-links a[aria-label='TikTok']:hover {
  color: #69c9d0;
}

.social-links a[aria-label='LinkedIn']:hover {
  color: #0a66c2;
}

.social-links a[aria-label='GitHub']:hover {
  color: #c0c0c0;
}

/* Responsive */
@media (max-width: 900px) {
  .left {
    width: 100vw;
    position: relative;
    height: 60vh;
  }

  .left-inner {
    height: 100%;
    padding-top: 100px;
    justify-content: flex-end;
    padding-bottom: 40px;
  }
}

@media (max-width: 600px) {
  .greeting {
    font-size: 1.6rem;
  }

  .description,
  .current-role {
    font-size: 1rem;
  }

  .social-links {
    gap: 16px;
  }

  .social-links a {
    width: 36px;
    height: 36px;
    font-size: 1.2rem;
  }
}
</style>
