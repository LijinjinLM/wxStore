<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
<h2><a id="user-content-安装" class="anchor" aria-hidden="true" href="#安装"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>安装</h2>
<h3><a id="user-content-方式一-通过-npm-安装-推荐" class="anchor" aria-hidden="true" href="#方式一-通过-npm-安装-推荐"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>方式一. 通过 npm 安装 (推荐)</h3>
<p>小程序已经支持使用 npm 安装第三方包，详见 <a href="https://developers.weixin.qq.com/miniprogram/dev/devtools/npm.html?search-key=npm" rel="nofollow">npm 支持</a></p>
<div class="highlight highlight-source-shell"><pre><span class="pl-c"><span class="pl-c">#</span> npm</span>
npm i vant-weapp -S --production

<span class="pl-c"><span class="pl-c">#</span> yarn</span>
yarn add vant-weapp --production</pre></div>
<h3><a id="user-content-方式二-下载代码" class="anchor" aria-hidden="true" href="#方式二-下载代码"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>方式二. 下载代码</h3>
<p>直接通过 git 下载 Vant Weapp 源代码，并将<code>dist</code>目录拷贝到自己的项目中</p>
<div class="highlight highlight-source-shell"><pre>git clone https://github.com/youzan/vant-weapp.git</pre></div>
<h2><a id="user-content-使用组件" class="anchor" aria-hidden="true" href="#使用组件"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>使用组件</h2>
<p>以按钮组件为例，只需要在 json 文件中引入按钮对应的自定义组件即可</p>
<div class="highlight highlight-source-json"><pre>{
  <span class="pl-s"><span class="pl-pds">"</span>usingComponents<span class="pl-pds">"</span></span>: {
    <span class="pl-s"><span class="pl-pds">"</span>van-button<span class="pl-pds">"</span></span>: <span class="pl-s"><span class="pl-pds">"</span>/path/to/vant-weapp/dist/button/index<span class="pl-pds">"</span></span>
  }
}</pre></div>
<p>接着就可以在 wxml 中直接使用组件</p>
<div class="highlight highlight-text-xml"><pre>&lt;<span class="pl-ent">van-button</span> <span class="pl-e">type</span>=<span class="pl-s"><span class="pl-pds">"</span>primary<span class="pl-pds">"</span></span>&gt;按钮&lt;/<span class="pl-ent">van-button</span>&gt;</pre></div>
<h2><a id="user-content-使用组件" class="anchor" aria-hidden="true" href="#使用组件"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>打包</h2>
<div class="highlight highlight-source-shell"><pre>npm install wepy-cli -g</pre><pre>git clone https://github.com/youzan/vant-weapp.git</pre></div>
  </body>
</html>

