# Noah Profile – Vue.js Portfolio

A modern, responsive developer portfolio built with Vue 3, Vite, and Framer Motion, designed to showcase skills, experience, and projects with elegant animations and a clean UI.

---

## 🚀 Features

- Modern Vue 3 + Vite stack
- Responsive design for desktop and mobile
- Animated transitions using [@vueuse/motion](https://motion.vueuse.org/)
- Framer Motion-inspired effects
- Social links with brand styling
- Project, Experience, Skills, and Education sections
- PDF resume download
- Vercel Analytics integration

---

## 📁 Project Structure

```
src/
  assets/           # Images, global CSS (main.css, Profile.png)
  components/
    LeftPanel.vue   # Left-side profile, intro, and social links
    RightPanel.vue  # Right-side: intro, skills, education, experience, projects, resume
  App.vue           # Main layout, imports panels
  main.js           # App entry, plugin setup
public/
  resume.pdf        # Downloadable resume (add your own)
  Profile.png       # Profile image
index.html          # Main HTML template, includes Vercel Analytics
```

---

## 🛠️ Tech Stack

- **Vue 3** – UI framework
- **Vite** – Fast build tool and dev server
- **@vueuse/motion** – Animations and transitions
- **Font Awesome** – Social/media icons
- **Vercel** – Hosting and analytics
- **CSS3** – Custom and responsive styling

---

## 📦 Installation

1. **Clone the repo:**
   ```sh
   git clone https://github.com/yourusername/vuejs-profile.git
   cd vuejs-profile
   ```

2. **Install dependencies:**
   ```sh
   npm install
   ```

3. **Run the development server:**
   ```sh
   npm run dev
   ```

4. **Build for production:**
   ```sh
   npm run build
   ```

---

## 🌐 Deployment

**Vercel** is recommended for seamless deployment:

1. Push your project to GitHub.
2. Import the repo on [vercel.com](https://vercel.com/).
3. Set the build command to `npm run build` and output directory to `dist`.
4. Add your `resume.pdf` and `Profile.png` to the `public/` folder.
5. Vercel Analytics is enabled via the script in `index.html`:
   ```html
   <script defer src="https://vercel.com/analytics/script.js"></script>
   ```

---

## 📄 Usage

- **Edit your profile and social links** in `LeftPanel.vue`.
- **Update your intro, skills, education, experience, and projects** in `RightPanel.vue`.
- **Replace `resume.pdf` and `Profile.png`** in the `public/` folder with your own files.

---

## ✨ Customization

- **Colors and gradients:** Edit in `main.css` and component `<style>` blocks.
- **Animations:** Tweak `motionVariants` in `RightPanel.vue` for custom effects.
- **Add more sections:** Duplicate and adapt the section structure in `RightPanel.vue`.

---

## 📑 License

MIT – use, modify, and share freely.

---

## 🙏 Credits

- [Vue.js](https://vuejs.org/)
- [Vite](https://vitejs.dev/)
- [@vueuse/motion](https://motion.vueuse.org/)
- [Font Awesome](https://fontawesome.com/)
- [Vercel](https://vercel.com/)

---

**Feel free to fork and make it your own!**