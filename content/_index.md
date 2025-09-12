---
title: Nirmanpreet Singh
layout: hextra-home
---

<style>
.social-tooltip {
  visibility: hidden;
  opacity: 0;
  position: absolute;
  left: 50%;
  top: -32px;
  transform: translateX(-50%);
  background: #222;
  color: #fff;
  padding: 4px 12px;
  border-radius: 8px;
  font-size: 0.95rem;
  white-space: nowrap;
  transition: opacity 0.2s;
  z-index: 10;
}
.social-icon:hover .social-tooltip,
.social-icon:focus .social-tooltip {
  visibility: visible;
  opacity: 1;
}
.feature-card-popup {
  position: relative;
  display: inline-block;
}
.popup-modal {
  display: none;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 90vw;
  max-width: 420px;
  min-width: 260px;
  min-height: 220px;
  background: rgba(34,34,34,0.70);
  color: #fff;
  border-radius: 24px;
  box-shadow: 0 12px 48px rgba(0,0,0,0.35);
  padding: 2rem 1.2rem 1.5rem 1.2rem;
  z-index: 100;
  backdrop-filter: blur(8px);
  border: 1px solid rgba(28,146,210,0.18);
  overflow-y: auto;
}
@media (max-width: 600px) {
  .popup-modal {
    padding: 1.2rem 0.5rem;
    max-width: 98vw;
    min-width: 0;
    font-size: 0.98rem;
  }
  .popup-close {
    top: 8px;
    right: 10px;
    width: 24px;
    height: 24px;
    font-size: 1rem;
  }
}
.popup-modal h1, .popup-modal h2, .popup-modal h3 {
  margin-top: 0;
  font-weight: 700;
  letter-spacing: 1px;
}
.popup-modal h2 {
  margin-top: 0;
  font-size: 1.3rem;
  font-weight: 700;
  margin-bottom: 0.7rem;
}
.popup-modal h3 {
  font-size: 1.08rem;
  margin-bottom: 0.5rem;
}
.popup-modal ul {
  margin-bottom: 1.2rem;
  padding-left: 1.2rem;
}
.popup-modal a {
  color: #1c92d2;
  font-weight: 600;
  text-decoration: underline;
  word-break: break-word;
}
.popup-close {
  position: absolute;
  top: 16px;
  right: 18px;
  background: #222;
  color: #fff;
  border: none;
  border-radius: 50%;
  width: 28px;
  height: 28px;
  font-size: 1.2rem;
  cursor: pointer;
  z-index: 101;
}
.feature-card-popup .card-tooltip {
  display: none;
  position: absolute;
  left: 50%;
  top: -32px;
  transform: translateX(-50%);
  background: #222;
  color: #fff;
  padding: 4px 12px;
  border-radius: 8px;
  font-size: 0.95rem;
  white-space: nowrap;
  z-index: 10;
}
.feature-card-popup:hover .card-tooltip,
.feature-card-popup:focus-within .card-tooltip {
  display: block;
}
</style>
<script>
class PopupManager {
  constructor() {
    this.openPopup = null;
    document.addEventListener('mousedown', (event) => {
      if (this.openPopup && this.openPopup.style.display === 'block') {
        if (!this.openPopup.contains(event.target) && !event.target.closest('.feature-card-popup')) {
          this.close();
        }
      }
    });
  }
  show(id) {
    if (this.openPopup) this.close();
    this.openPopup = document.getElementById(id);
    if (this.openPopup) {
      this.openPopup.style.display = 'block';
      document.body.classList.add('popup-open');
    }
  }
  close() {
    if (this.openPopup) {
      this.openPopup.style.display = 'none';
      document.body.classList.remove('popup-open');
      this.openPopup = null;
    }
  }
}
window.popupManager = new PopupManager();
</script>

<div class="hx:w-full hx:flex hx:flex-col hx:items-center hx:justify-center hx:mt-8 hx:relative">
  <div class="hx:relative" style="width:160px;height:160px;">
    <img src="https://gravatar.com/avatar/bfd1ed7dab854d1aa5f5c755114da46ccb6c85648373ed876eb322d4876fa731?v=1639790166000&size=120&d=initials"
      alt="Avatar"
      width="100"
      height="100"
      class="hx:rounded-full hx:shadow-lg"
      style="position:absolute;left:50%;top:50%;transform:translate(-50%,-50%);z-index:2;"
    >
    <!-- Top (0°) -->
    <a href="https://github.com/nirmanpreet" target="_blank"
       class="social-icon hx:bg-gray-800 hx:rounded-full hx:p-2 hx:flex hx:items-center hx:justify-center hx:shadow hx:transition hover:hx:bg-primary-400 hx:absolute"
       style="left:50%;top:0;transform:translate(-50%,-50%);z-index:3;">
      {{< icon name="github" attributes="height=24" >}}
      <span class="social-tooltip">Visit my Github</span>
    </a>
    <!-- Right (90°) -->
    <a href="https://instagram.com/yourusername" target="_blank"
       class="social-icon hx:bg-gray-800 hx:rounded-full hx:p-2 hx:flex hx:items-center hx:justify-center hx:shadow hx:transition hover:hx:bg-primary-400 hx:absolute"
       style="left:100%;top:50%;transform:translate(-50%,-50%);z-index:3;">
      {{< icon name="instagram" attributes="height=24" >}}
      <span class="social-tooltip">Visit my Instagram</span>
    </a>
    <!-- Bottom (180°) -->
    <a href="mailto:nirmanpreet@gmail.com"
       class="social-icon hx:bg-gray-800 hx:rounded-full hx:p-2 hx:flex hx:items-center hx:justify-center hx:shadow hx:transition hover:hx:bg-primary-400 hx:absolute"
       style="left:50%;top:100%;transform:translate(-50%,-50%);z-index:3;">
      {{< icon name="mail" attributes="height=24" >}}
      <span class="social-tooltip">Send me an Email</span>
    </a>
    <!-- Left (270°) -->
    <a href="https://linkedin.com/in/yourusername" target="_blank"
       class="social-icon hx:bg-gray-800 hx:rounded-full hx:p-2 hx:flex hx:items-center hx:justify-center hx:shadow hx:transition hover:hx:bg-primary-400 hx:absolute"
       style="left:0;top:50%;transform:translate(-50%,-50%);z-index:3;">
      {{< icon name="linkedin" attributes="height=24" >}}
      <span class="social-tooltip">Visit my LinkedIn</span>
    </a>
  </div>
  <h1 class="hx:mt-8 hx:text-4xl hx:font-bold hx:text-center">Nirmanpreet Singh</h1>
  <h2 class="hx:text-xl hx:font-semibold hx:mt-2 hx:text-center">Aspiring Software Developer & Cybersecurity Enthusiast</h2>
  <div class="hx:mt-2 hx:text-lg hx:text-center">Bachelor of Information Technology</div>
  <div class="hx:text-base hx:text-gray-400 hx:mb-4 hx:text-center">Focused on secure software development, ethical hacking, and cyber defense.</div>
  <div class="hx:mb-6 hx:flex hx:gap-4 hx:justify-center">
  {{< hextra/hero-button text="Read My Blog" link="blog" >}}
  {{< hextra/hero-button text="View Projects" link="projects" >}}
  {{< hextra/hero-button text="Download Resume" link="resume.pdf" >}}
</div>
</div>
{{< bloghighlight >}}
{{< hextra/feature-grid >}}
  <!-- Skills Card -->
  <div class="feature-card-popup" style="position:relative;">
    <span class="card-tooltip">Click to view more</span>
    <div onclick="popupManager.show('skills-popup')" style="cursor:pointer;">
      {{< hextra/feature-card
        title="Skills"
        subtitle="Python, Linux, Network Security, Web Application Security, JavaScript, Ethical Hacking"
        icon="code"
        style="background: radial-gradient(ellipse at 50% 80%,rgba(28,146,210,0.10),hsla(0,0%,100%,0));"
      >}}
    </div>
    <div class="popup-modal" id="skills-popup">
      <button class="popup-close" onclick="popupManager.close()">&times;</button>
      <h2>🚀 Skills Overview</h2>
      <p><strong>Core skillset for software and cybersecurity roles:</strong></p>
      <h3>🛠️ Technical Skills</h3>
      <ul>
        <li><strong>Python:</strong> Scripting, automation, security tools</li>
        <li><strong>Linux:</strong> Server management, hardening, bash scripting</li>
        <li><strong>Network Security:</strong> Firewalls, IDS/IPS, secure protocols</li>
        <li><strong>Web Application Security:</strong> OWASP Top 10, penetration testing</li>
        <li><strong>JavaScript:</strong> Frontend & backend development</li>
        <li><strong>Ethical Hacking:</strong> CTFs, vulnerability assessment</li>
      </ul>
      <div style="background:rgba(28,146,210,0.10);padding:0.7em 1em;border-radius:8px;margin-bottom:1em;">
        <strong>TIP:</strong> I regularly participate in CTFs and open source security projects.
      </div>
      <h3>📚 Related Projects</h3>
      <ul>
        <li><a href='projects'>SecureChat</a>: Encrypted messaging app</li>
        <li><a href='projects'>VulnScanner</a>: Automated vulnerability scanner</li>
        <li><a href='projects'>Linux Fortress</a>: Hardening scripts</li>
      </ul>
      <p>See my <a href="projects">full portfolio</a> or <a href="blog">read my blog</a> for more!</p>
    </div>
  </div>
  <!-- Projects Card -->
  <div class="feature-card-popup" style="position:relative;">
    <span class="card-tooltip">Click to view more</span>
    <div onclick="popupManager.show('projects-popup')" style="cursor:pointer;">
      {{< hextra/feature-card
        title="Projects"
        subtitle="SecureChat: Encrypted messaging app | VulnScanner: Automated vulnerability scanner | Linux Fortress: Hardening scripts | CTF Writeups: Published solutions for security challenges"
        icon="terminal"
        style="background: radial-gradient(ellipse at 50% 80%,rgba(221,210,59,0.10),hsla(0,0%,100%,0));"
      >}}
    </div>
    <div class="popup-modal" id="projects-popup">
      <button class="popup-close" onclick="popupManager.close()">&times;</button>
      <h2>🧑‍💻 Project Highlights</h2>
      <ul>
        <li><strong>SecureChat:</strong> Real-time encrypted chat app with user authentication and group messaging.</li>
        <li><strong>VulnScanner:</strong> Automated tool for scanning web apps for vulnerabilities, with detailed reporting.</li>
        <li><strong>Linux Fortress:</strong> Bash scripts for server hardening, firewall setup, and intrusion detection.</li>
        <li><strong>CTF Writeups:</strong> Step-by-step solutions for reverse engineering, cryptography, and web exploits.</li>
      </ul>
      <div style="background:rgba(221,210,59,0.10);padding:0.7em 1em;border-radius:8px;margin-bottom:1em;">
        <strong>NOTE:</strong> All projects are open source and available on my <a href="https://github.com/nirmanpreet">GitHub</a>.
      </div>
      <p>Explore more on my <a href="projects">projects page</a> or <a href="blog">read my blog</a> for technical deep-dives.</p>
    </div>
  </div>
  <!-- Education Card -->
  <div class="feature-card-popup" style="position:relative;">
    <span class="card-tooltip">Click to view more</span>
    <div onclick="popupManager.show('education-popup')" style="cursor:pointer;">
      {{< hextra/feature-card
        title="Education"
        subtitle="Bachelor of Information Technology (Cybersecurity & Software Development Focus), Graduated 2025"
        icon="academic-cap"
        style="background: radial-gradient(ellipse at 50% 80%,rgba(142,53,74,0.10),hsla(0,0%,100%,0));"
      >}}
    </div>
    <div class="popup-modal" id="education-popup">
      <button class="popup-close" onclick="popupManager.close()">&times;</button>
      <h2>🎓 Education</h2>
      <ul>
        <li><strong>Bachelor of Information Technology</strong></li>
        <li>Major: Cybersecurity & Software Development</li>
        <li>Graduated: 2025</li>
        <li>Relevant Coursework: Secure Coding, Network Security, Cloud Computing, Data Structures</li>
      </ul>
      <div style="background:rgba(142,53,74,0.10);padding:0.7em 1em;border-radius:8px;margin-bottom:1em;">
        <strong>TIP:</strong> Completed multiple hands-on labs and capstone projects in cyber defense.
      </div>
      <p>See my <a href="blog">blog</a> for study tips and university experiences.</p>
    </div>
  </div>
  <!-- Certifications Card -->
  <div class="feature-card-popup" style="position:relative;">
    <span class="card-tooltip">Click to view more</span>
    <div onclick="popupManager.show('certifications-popup')" style="cursor:pointer;">
      {{< hextra/feature-card
        title="Certifications"
        subtitle="CompTIA Security+ (in progress), Cisco CyberOps Associate (in progress)"
        style="background: radial-gradient(ellipse at 50% 80%,rgba(97,194,254,0.10),hsla(0,0%,100%,0));"
      >}}
    </div>
    <div class="popup-modal" id="certifications-popup">
      <button class="popup-close" onclick="popupManager.close()">&times;</button>
      <h2>📜 Certifications</h2>
      <ul>
        <li><strong>CompTIA Security+</strong> (in progress)</li>
        <li><strong>Cisco CyberOps Associate</strong> (in progress)</li>
        <li><strong>Linux Foundation Certified IT Associate</strong> (planned)</li>
      </ul>
      <div style="background:rgba(97,194,254,0.10);padding:0.7em 1em;border-radius:8px;margin-bottom:1em;">
        <strong>NOTE:</strong> I am committed to continuous learning and professional development.
      </div>
      <p>Check my <a href="blog">blog</a> for certification study guides and tips.</p>
    </div>
  </div>
  <!-- Interests Card -->
  <div class="feature-card-popup" style="position:relative;">
    <span class="card-tooltip">Click to view more</span>
    <div onclick="popupManager.show('interests-popup')" style="cursor:pointer;">
      {{< hextra/feature-card
        title="Interests"
        subtitle="Cybersecurity, Open Source, Capture The Flag, Secure Coding, Cloud Security"
        icon="sparkles"
        style="background: radial-gradient(ellipse at 50% 80%,rgba(194,97,254,0.10),hsla(0,0%,100%,0));"
      >}}
    </div>
    <div class="popup-modal" id="interests-popup">
      <button class="popup-close" onclick="popupManager.close()">&times;</button>
      <h2>🌟 Interests</h2>
      <ul>
        <li>Cybersecurity research and bug bounty hunting</li>
        <li>Open source contributions (security tools)</li>
        <li>Capture The Flag competitions</li>
        <li>Cloud security and automation</li>
        <li>Secure coding practices</li>
      </ul>
      <div style="background:rgba(194,97,254,0.10);padding:0.7em 1em;border-radius:8px;margin-bottom:1em;">
        <strong>TIP:</strong> I love collaborating with global teams and learning new tech!
      </div>
      <p>Read more about my interests on my <a href="blog">blog</a>.</p>
    </div>
  </div>
  <!-- Recommendations Card -->
  <div class="feature-card-popup" style="position:relative;">
    <span class="card-tooltip">Click to view more</span>
    <div onclick="popupManager.show('recommendations-popup')" style="cursor:pointer;">
      {{< hextra/feature-card
        title="Recommendations"
        subtitle="\"Nirmanpreet is a dedicated learner and a creative problem solver. His passion for cybersecurity and software development is evident in his projects and teamwork. Highly recommended for any tech-driven role.\" — Mentor\n\"Consistently delivers secure, high-quality code and demonstrates strong leadership in group projects.\" — Peer"
        icon="chat"
        style="background: radial-gradient(ellipse at 50% 80%,rgba(53,142,74,0.10),hsla(0,0%,100%,0));"
      >}}
    </div>
    <div class="popup-modal" id="recommendations-popup">
      <button class="popup-close" onclick="popupManager.close()">&times;</button>
      <h2>💬 Recommendations</h2>
      <ul>
        <li><strong>Mentor:</strong> "Nirmanpreet is a dedicated learner and a creative problem solver. His passion for cybersecurity and software development is evident in his projects and teamwork. Highly recommended for any tech-driven role."</li>
        <li><strong>Peer:</strong> "Consistently delivers secure, high-quality code and demonstrates strong leadership in group projects."</li>
        <li><strong>Professor:</strong> "Shows initiative and curiosity in every assignment, especially in security labs."</li>
      </ul>
      <div style="background:rgba(53,142,74,0.10);padding:0.7em 1em;border-radius:8px;margin-bottom:1em;">
        <strong>NOTE:</strong> References available upon request.
      </div>
      <p>See more feedback and testimonials on my <a href="blog">blog</a>.</p>
    </div>
  </div>
{{< /hextra/feature-grid >}}