---
layout: page
title: Contact
permalink: /contact/
---

<section class="contact" itemscope itemtype="https://schema.org/Person">
  <meta itemprop="name" content="Jieyang Hu">

  <h2>Contact Information</h2>

  <ul class="contact-list">
    <li>
      <i class="fa fa-map-marker" aria-hidden="true"></i>
      <span class="label">Address</span>
      <a itemprop="address" href="https://maps.google.com/?q=No.96+Jinzhai+Road,+Hefei,+Anhui,+China+230026" target="_blank" rel="noopener">
        No.96 Jinzhai Road, Hefei, Anhui, China 230026
      </a>
    </li>

    <li>
      <i class="fa fa-envelope" aria-hidden="true"></i>
      <span class="label">Email</span>
      <a href="mailto:jieyanghu@mail.ustc.edu.cn">jieyanghu@mail.ustc.edu.cn</a>
    </li>

    <li>
      <i class="fa fa-qq" aria-hidden="true"></i>
      <span class="label">QQ</span>
      <span class="mono">2174214603</span>
    </li>

    <!-- 可选：学术图标（注释去掉并填写你的ID） -->
    <!--
    <li>
      <i class="ai ai-google-scholar"></i>
      <span class="label">Google Scholar</span>
      <a href="https://scholar.google.com/citations?user=YOUR_ID" target="_blank" rel="noopener">Profile</a>
    </li>
    <li>
      <i class="ai ai-orcid"></i>
      <span class="label">ORCID</span>
      <a href="https://orcid.org/0000-0000-0000-0000" target="_blank" rel="noopener">0000-0000-0000-0000</a>
    </li>
    <li>
      <i class="fa fa-github"></i>
      <span class="label">GitHub</span>
      <a href="https://github.com/jerryh0502" target="_blank" rel="noopener">jerryh0502</a>
    </li>
    -->
  </ul>
</section>

<style>
/* 样式适配暗色模式 */
.contact { margin-top: 0.5rem; }
.contact-list { list-style: none; padding: 0; margin: 0; display: grid; gap: .75rem; }
.contact-list li { display: grid; grid-template-columns: 1.25rem auto 1fr; align-items: center; gap: .6rem; }
.contact-list i { opacity: .9; }
.contact-list .label { font-weight: 600; min-width: 5.5rem; color: var(--muted, #666); }
.contact-list a { text-decoration: none; border-bottom: 1px dashed rgba(127,127,127,.35); }
.contact-list a:hover { border-bottom-style: solid; }
.mono { font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", monospace; }
@media (max-width: 560px) {
  .contact-list li { grid-template-columns: 1.25rem 5.5rem 1fr; align-items: start; }
}
</style>
