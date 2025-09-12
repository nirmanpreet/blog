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
  {{< hextra/hero-button text="Download Resume" link="resume.pdf" >}}
</div>
</div>


{{< latest-updates >}}