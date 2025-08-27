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
      <span id="email" class="mono" data-user="jieyanghu" data-host="mail.ustc.edu.cn">[protected]</span>
      <button id="copy-email" class="ghost-btn" aria-label="Copy email">Copy</button>
      <a id="mailto-link" class="ghost-btn" aria-label="Open mail" href="#" rel="nofollow">Mail</a>
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
/* 轻量样式：跟随站点的暗/亮色（尽量用变量，若无变量也能正常显示） */
.contact { margin-top: 0.5rem; }
.contact-list { list-style: none; padding: 0; margin: 0; display: grid; gap: .75rem; }
.contact-list li { display: grid; grid-template-columns: 1.25rem auto 1fr; align-items: center; gap: .6rem; }
.contact-list i { opacity: .9; }
.contact-list .label { font-weight: 600; min-width: 5.5rem; color: var(--muted, #666); }
.contact-list a { text-decoration: none; border-bottom: 1px dashed rgba(127,127,127,.35); }
.contact-list a:hover { border-bottom-style: solid; }
.mono { font-family: ui-monospace, SFMono-Regular, Menlo, Monaco, Consolas, "Liberation Mono", monospace; }
.ghost-btn {
  margin-left: .4rem; padding: .25rem .5rem; font-size: .8rem; border-radius: .6rem;
  border: 1px solid rgba(127,127,127,.35); background: transparent; cursor: pointer;
}
.ghost-btn:hover { border-color: rgba(127,127,127,.6); }
@media (max-width: 560px) {
  .contact-list li { grid-template-columns: 1.25rem 5.5rem 1fr; align-items: start; }
}
</style>

<script>
/* 轻量防爬：运行时拼邮箱；并提供复制与 mailto */
(function(){
  const span = document.getElementById('email');
  if(!span) return;
  const user = span.dataset.user, host = span.dataset.host;
  const addr = user + '@' + host;
  span.textContent = addr;
  const mailto = document.getElementById('mailto-link');
  if (mailto) mailto.href = 'mailto:' + addr;

  const copyBtn = document.getElementById('copy-email');
  if (copyBtn) {
    copyBtn.addEventListener('click', async () => {
      try {
        await navigator.clipboard.writeText(addr);
        copyBtn.textContent = 'Copied!';
        setTimeout(()=>copyBtn.textContent='Copy', 1400);
      } catch(e) {
        copyBtn.textContent = 'Press ⌘/Ctrl+C';
        setTimeout(()=>copyBtn.textContent='Copy', 2000);
      }
    });
  }
})();
</script>
