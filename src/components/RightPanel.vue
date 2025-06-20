<template>
  <div class="right">
    <div class="right-inner">
      <transition name="fade" appear>
        <section class="intro-section">
          <h4 class="section-title">Intro</h4>
          <p>
            I'm an enthusiastic and adaptable web developer based in Nairobi, KENYA, with two years
            of experience building responsive and scalable web applications using modern
            technologies.
          </p>
          <p>
            I enjoy being the bridge between engineering and design, and feel right at home as a
            front end engineer. Driven by a passion for creating impactful solutions, I thrive on
            learning and tackling new challenges. I'm committed to leveraging technology to make a
            real difference. I'm experienced in developing and designing products for the web, from
            simple landing pages to full-fledged web apps.
          </p>
          <p>
            Always open to discussing new projects, creative ideas, or opportunities to be part of
            your visions.
          </p>
        </section>
      </transition>

      <section v-motion="motionVariants" class="skills-section card-glass">
        <h4 class="section-title">Skills</h4>
        <div class="skills-content">
          <div class="skill-line">
            <strong>LANGUAGES:</strong> JavaScript (ES6), HTML5, CSS3, Java, Python, TypeScript,
            React, Node.js, Next.js, Express.js, Bootstrap5, TailwindCSS
          </div>
          <div class="skill-line">
            <strong>LIBRARIES & FRAMEWORKS:</strong> jQuery, Bootstrap, Node, MongoDB, Express,
            React
          </div>
          <div class="skill-line">
            <strong>TOOLS:</strong> Git & Github, AWS Command Line, VS Code, Postman, Figma, Docker,
            Vercel, Netlify, Jira, Trello
          </div>
        </div>
      </section>

      <section
        v-motion="{
          initial: motionVariants.initial,
          enter: { ...motionVariants.enter, transition: { delay: 0.15 } },
        }"
        class="education card-glass"
      >
        <h4 class="section-title">Education</h4>
        <div class="content">
          <div class="education-item">
            <h3 class="university">CHUKA UNIVERSITY</h3>
            <p class="college">Bachelor of Science in Applied Computer Science</p>

            <div class="education-details">
              <div class="detail-item"><strong>Major:</strong> Applied Science</div>
              <div class="detail-item">
                <strong>Concentration:</strong> Human Computer Interaction, Web Development, Mobile
                App Development
              </div>
            </div>

            <div class="grad-date">Expected Graduation: Nov 2025</div>
          </div>
        </div>
      </section>

      <section
        v-motion="{
          initial: motionVariants.initial,
          enter: { ...motionVariants.enter, transition: { delay: 0.3 } },
        }"
        class="experience card-glass"
      >
        <h4 class="section-title">Experience</h4>
        <div class="content">
          <div class="exp-item">
            <div class="exp-header">
              <div class="job-info">
                <h3 class="company">Fusional Tech</h3>
                <p class="job-title">Software Engineer Co-op</p>
              </div>
              <div class="duration">June 2025 – Present</div>
            </div>

            <ul class="description">
              <li>
                Built major features of Fusional's customer-facing app with Vue.js, Tailwind CSS,
                Node.js, and REST APIs
              </li>
              <li>Proposed and implemented user-centered designs across web/mobile apps</li>
              <li>Engineered cloud services interacting with internal & external APIs</li>
            </ul>
          </div>

          <div class="exp-item">
            <div class="exp-header">
              <div class="job-info">
                <h3 class="company">Freelance</h3>
                <p class="job-title">Freelance Web Developer</p>
              </div>
              <div class="duration">Jan 2023 – Present</div>
            </div>

            <ul class="description">
              <li>Developed responsive apps with Vue.js, React, Angular</li>
              <li>Delivered custom client solutions for business needs</li>
              <li>Optimized for performance & UX best practices</li>
            </ul>
          </div>

          <div class="exp-item">
            <div class="exp-header">
              <div class="job-info">
                <h3 class="company">Electratech Innovation Limited (ETI)</h3>
                <p class="job-title">Web Developer  Intern</p>
              </div>
              <div class="duration">May 2024 – September 2024</div>
            </div>
            <ul class="description">
              <li>
                Performed routine system maintenance, including updates, bug fixes, and optimization
                of hardware components.
              </li>
              <li>
                Provided technical support to staff and clients, addressing issues related to
                operating systems, network connectivity.
              </li>
              <li>
                Collaborated with senior developers to design, build, and maintain responsive and
                user-friendly websites.
              </li>
              <li>
                Digital and audience marketing through managing and optimizing social media accounts
                and email marketing campaigns.
              </li>
              
            </ul>
          </div>
        </div>
      </section>

      <transition name="fade" appear>
        <section
         v-motion="{
          initial: motionVariants.initial,
          enter: { ...motionVariants.enter, transition: { delay: 0.3 } },
        }"
        class="experience card-glass"
      >
          <h4 class="section-title">PROJECTS</h4>
          <div class="projects-list">
            <div class="project-item">
              <h5 class="project-title">Portfolio Website</h5>
              <p class="project-desc">
                A personal portfolio built with JavaScript, React.js, Tailwind CSS, and Framer
                Motion, deployed on Vercel.
              </p>
            </div>
            <div class="project-item">
              <h5 class="project-title">Fusional Tech Agency</h5>
              <p class="project-desc">
                IT consultancy website built in NextJS, featuring SEO optimization, Google indexing,
                tag manager, and analytics.
              </p>
            </div>
            <div class="project-item">
              <h5 class="project-title">Learning Management System</h5>
              <p class="project-desc">
                A web-based platform for online education and training, offering course management,
                user authentication, progress tracking, and interactive content. Built for
                scalability and ease of use for both instructors and students.
              </p>
            </div>
            <div class="project-item">
              <h5 class="project-title">AI-Image Gen</h5>
              <p class="project-desc">
                An advanced image generation tool leveraging artificial intelligence to create
                high-quality visuals based on user input.
              </p>
            </div>
            <div class="project-item">
              <h5 class="project-title">Car-Rental System</h5>
              <p class="project-desc">
                A dynamic and user-friendly Car Rental System built using PHP and MySQL, designed to
                streamline the process of renting vehicles online.
              </p>
            </div>
          </div>
        </section>
      </transition>

      <div class="resume-link-container">
        <a href="/resume.pdf" target="_blank" rel="noopener" class="resume-link">
          GRAB A PDF OF MY FULL RESUME
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>
const motionVariants = {
  initial: { opacity: 0, y: 50 },
  enter: {
    opacity: 1,
    y: 0,
    transition: {
      type: 'spring',
      stiffness: 250,
      damping: 22,
    },
  },
}
</script>

<style scoped>
.right {
  width: 50vw;
  min-height: 100vh;
  margin-left: 50vw;
  background: #fff;
  display: flex;
  align-items: flex-start;
  justify-content: center;
  padding: 40px 0;
  box-sizing: border-box;
}

.right-inner {
  width: 90%;
  max-width: 800px;
}

.card-glass {
  background: rgba(255, 255, 255, 0.8);
  border-radius: 12px;
  box-shadow: 0 8px 30px rgba(0, 0, 0, 0.1);
  padding: 25px 30px;
  margin-bottom: 40px;
  backdrop-filter: blur(8px);
  transition: transform 0.3s ease;
}

.card-glass:hover {
  transform: translateY(-5px);
}

.section-title {
  font-size: 1.4rem;
  font-weight: 600;
  margin-bottom: 20px;
  color: #2c3e50;
}

.skill-line {
  margin-bottom: 12px;
  font-size: 1.05rem;
  color: #2d3436;
}

.education-item,
.exp-item {
  padding: 12px 0;
}

.university {
  font-size: 1.1rem;
  font-weight: 700;
  color: #34495e;
}

.company {
  font-size: 1.1rem;
  font-weight: bold;
  color: #2c3e50;
}

.job-title {
  font-size: 0.98rem;
  color: #7f8c8d;
}

.duration {
  font-size: 0.9rem;
  background: #ecf0f1;
  padding: 4px 10px;
  border-radius: 20px;
  color: #2c3e50;
  text-transform: uppercase;
}

.description {
  list-style: none;
  padding: 0;
  margin-top: 10px;
}

.description li {
  margin-bottom: 10px;
  padding-left: 20px;
  position: relative;
  font-size: 0.95rem;
  color: #333;
}

.description li::before {
  content: '•';
  position: absolute;
  left: 0;
  color: #4facfe;
  font-size: 1.2rem;
}

.projects-section {
  margin-bottom: 40px;
}
.section-title {
  font-size: 1.3rem;
  margin-bottom: 16px;
  color: #2c3e50;
  font-weight: 700;
  letter-spacing: 1px;
}
.projects-list {
  display: flex;
  flex-direction: column;
  gap: 24px;
}
.project-item {
  background: #f8f9fa;
  border-radius: 10px;
  padding: 18px 20px;
  box-shadow: 0 2px 8px rgba(44, 62, 80, 0.04);
}
.project-title {
  font-size: 1.1rem;
  font-weight: 600;
  margin-bottom: 6px;
  color: #1abc5b;
}
.project-desc {
  font-size: 1rem;
  color: #444;
  margin-bottom: 0;
}

.resume-link-container {
  margin-top: 40px;
  display: flex;
  justify-content: center;
}

.resume-link {
  display: block;
  width: 100%;
  max-width: 95%;
  padding: 18px 0;
  background: #b7e4bb;
  border-radius: 10px;
  text-align: center;
  font-size: 1.35rem;
  font-weight: 600;
  letter-spacing: 1px;
  color: #0e7c3a;
  text-decoration: none;
  transition:
    background 0.2s,
    color 0.2s;
  background-clip: padding-box;
  margin: 0 auto;
}

.resume-link:hover {
  background: #c8e6c9;
  color: #1a66bc;
}

@media (max-width: 900px) {
  .right {
    width: 100vw;
    margin-left: 0;
    padding: 30px 0;
  }
  .right-inner {
    width: 95%;
  }
}

@media (max-width: 600px) {
  .section-title {
    font-size: 1.2rem;
  }
  .skill-line,
  .description li {
    font-size: 0.9rem;
  }
  .university,
  .company {
    font-size: 1rem;
  }
  .duration {
    font-size: 0.8rem;
    padding: 2px 8px;
  }
}
</style>
