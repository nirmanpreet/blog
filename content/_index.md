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
  transform: translate(-40%, -50%);
  width: 380px;
  min-height: 220px;
  background: rgba(34,34,34,0.40); /* translucent */
  color: #fff;
  border-radius: 24px;
  box-shadow: 0 12px 48px rgba(0,0,0,0.35);
  padding: 2rem 2rem 1.5rem 2rem;
  z-index: 100;
  backdrop-filter: blur(8px);
  border: 1px solid rgba(28,146,210,0.18);
}
.popup-modal h3 {
  margin-top: 0;
  font-size: 1.4rem;
  font-weight: 700;
  letter-spacing: 1px;
  margin-bottom: 1rem;
}
.popup-modal ul {
  margin-bottom: 1.2rem;
  padding-left: 1.2rem;
}
.popup-modal a {
  color: #1c92d2;
  font-weight: 600;
  text-decoration: underline;
}
.feature-card-popup:hover .popup-modal,
.feature-card-popup:focus-within .popup-modal {
  display: block;
}
</style>

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
</div>
</div>


{{< hextra/feature-grid >}}
  <div class="feature-card-popup">
    {{< hextra/feature-card
      title="Skills"
      subtitle="Python, Linux, Network Security, Web Application Security, JavaScript, Ethical Hacking"
      icon="code"
      style="background: radial-gradient(ellipse at 50% 80%,rgba(28,146,210,0.10),hsla(0,0%,100%,0));"
    >}}
    <div class="popup-modal">
      <h3>Skills Details</h3>
      <ul>
        <li>Python: Scripting, automation, and security tools</li>
        <li>Linux: Server management, hardening, and bash scripting</li>
        <li>Network Security: Firewalls, IDS/IPS, and secure protocols</li>
        <li>Web Application Security: OWASP Top 10, penetration testing</li>
        <li>JavaScript: Frontend and backend development</li>
        <li>Ethical Hacking: CTFs, vulnerability assessment</li>
      </ul>
      <a href='projects'>See related projects</a>
    </div>
  </div>
  {{< hextra/feature-card
    title="Projects"
    subtitle="SecureChat: Encrypted messaging app | VulnScanner: Automated vulnerability scanner | Linux Fortress: Hardening scripts | CTF Writeups: Published solutions for security challenges"
    icon="terminal"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(221,210,59,0.10),hsla(0,0%,100%,0));"
  >}}
  {{< hextra/feature-card
    title="Education"
    subtitle="Bachelor of Information Technology (Cybersecurity & Software Development Focus), Graduated 2025"
    icon="academic-cap"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(142,53,74,0.10),hsla(0,0%,100%,0));"
  >}}
  {{< hextra/feature-card
    title="Certifications"
    subtitle="CompTIA Security+ (in progress), Cisco CyberOps Associate (in progress)"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(97,194,254,0.10),hsla(0,0%,100%,0));"
  >}}
  {{< hextra/feature-card
    title="Interests"
    subtitle="Cybersecurity, Open Source, Capture The Flag, Secure Coding, Cloud Security"
    icon="sparkles"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(194,97,254,0.10),hsla(0,0%,100%,0));"
  >}}
  {{< hextra/feature-card
    title="Recommendations"
    subtitle="\"Nirmanpreet is a dedicated learner and a creative problem solver. His passion for cybersecurity and software development is evident in his projects and teamwork. Highly recommended for any tech-driven role.\" — Mentor\n\"Consistently delivers secure, high-quality code and demonstrates strong leadership in group projects.\" — Peer"
    icon="chat"
    style="background: radial-gradient(ellipse at 50% 80%,rgba(53,142,74,0.10),hsla(0,0%,100%,0));"
  >}}
{{< /hextra/feature-grid >}}