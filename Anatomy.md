<!DOCTYPE html>
<html lang="en"><head>
  <meta charset="utf-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1"><!-- Begin Jekyll SEO tag v2.9.0 -->
<title>Anatomy of GitHub Pages | Open Coding</title>
<meta name="generator" content="Jekyll v3.9.5" />
<meta property="og:title" content="Anatomy of GitHub Pages" />
<meta property="og:locale" content="en_US" />
<meta name="description" content="Learn the Files and development work flow of GitHub Pages. This includes working with you home page, theme, markdown, and more." />
<meta name="twitter:description" property="og:description" content="Learn the Files and development work flow of GitHub Pages. This includes working with you home page, theme, markdown, and more." />
<meta property="og:site_name" content="Open Coding" />
<meta property="og:type" content="article" />
<meta property="article:published_time" content="2023-08-24T00:00:00+00:00" />
<meta property="article:modified_time" content="2023-08-24T00:00:00+00:00" />
<meta name="twitter:card" content="summary" />
<meta name="twitter:title" content="Anatomy of GitHub Pages" />
<script type="application/ld+json">
{"@context":"https://schema.org","@type":"BlogPosting","dateModified":"2023-08-24T00:00:00+00:00","datePublished":"2023-08-24T00:00:00+00:00","description":"Learn the Files and development work flow of GitHub Pages. This includes working with you home page, theme, markdown, and more.","headline":"Anatomy of GitHub Pages","mainEntityOfPage":{"@type":"WebPage","@id":"/github/pages/anatomy"},"url":"/github/pages/anatomy"}</script>
<!-- End Jekyll SEO tag -->
<link id="main-stylesheet" rel="stylesheet" href="/assets/css/style.css"><link type="application/atom+xml" rel="alternate" href="/feed.xml" title="Open Coding" />
<!-- Minima start custom head snippets -->
<!-- Favicon for browser tabs and bookmarks -->
<link rel="icon" href="/favicon.ico" type="image/x-icon">

<!-- Support for Apple devices (iPhone/iPad homescreen icon) -->
<link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png">

<!-- Support for modern browsers and pinned tabs -->
<link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png">
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">

<!-- Google Fonts - commonly used across the site -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Roboto:wght@400;500;700&family=Open+Sans:wght@400;600&family=Lato:wght@400;700&family=Montserrat:wght@400;600&family=Noto+Sans:wght@400;700&family=Merriweather:wght@400;700&family=Source+Code+Pro:wght@400;700&family=Orbitron:wght@400;700;900&family=Rajdhani:wght@300;400;600;700&family=Press+Start+2P&display=swap" rel="stylesheet"><link rel="stylesheet" href="/assets/css/style.css">
<script src="/assets/js/user-preferences.js"></script>
<!-- Set up javaURI globally for OCS Analytics Tracker -->
<script>
    if (location.hostname === "localhost" || location.hostname === "127.0.0.1") {
        window.javaURI = "http://localhost:8585";
    } else {
        window.javaURI = "https://spring.opencodingsociety.com";
    }
</script>
<!-- OCS Analytics Tracking Script (loaded on every page) -->
<script src="/assets/js/ocs-analytics-tracker.js" defer></script>
<!-- Keyboard Shortcuts (Alt+Shift+key navigation, loaded on every page) -->
<script>window.baseurl = "";</script>
<script src="/assets/js/keyboard-shortcuts.js" defer></script>

<!-- AI A/B Test Engine SDK (passes site.baseurl for asset resolution) -->
<script src="https://ai-ab-test-engine.vercel.app/sdk.js"
  data-site-baseurl=""
  data-project-id="cmnfour780000f63gu69kg2v8"></script>
<script type="importmap">
{
  "imports": {
    "@assets/": "/assets/",
    "@fortuneFinders/": "/assets/js/fortuneFinders/"
  }
}
</script>

<!-- Minima end custom head snippets -->
 </head>
<body>    <header class="site-header">
        <div class="wrapper"><a class="site-title" rel="author" href="/" data-value="Open Coding">
                <img id="site-logo" src="/images/logo.png" alt="Logo">
            </a><nav class="site-nav">
                <input type="checkbox" id="nav-trigger" class="nav-trigger" />
                <label for="nav-trigger">
                    <span class="menu-icon">
                        <svg viewBox="0 0 18 15" width="18px" height="15px">
                            <path
                                d="M18,1.484c0,0.82-0.665,1.484-1.484,1.484H1.484C0.665,2.969,0,2.304,0,1.484l0,0C0,0.665,0.665,0,1.484,0 h15.032C17.335,0,18,0.665,18,1.484L18,1.484z M18,7.516C18,8.335,17.335,9,16.516,9H1.484C0.665,9,0,8.335,0,7.516l0,0 c0-0.82,0.665-1.484,1.484-1.484h15.032C17.335,6.031,18,6.696,18,7.516L18,7.516z M18,13.516C18,14.335,17.335,15,16.516,15H1.484 C0.665,15,0,14.335,0,13.516l0,0c0-0.82,0.665-1.483,1.484-1.483h15.032C17.335,12.031,18,12.695,18,13.516L18,13.516z" />
                        </svg>
                    </span>
                </label>

                <div class="trigger"><a class="page-link" href="/navigation/blogs/">Blogs</a><a class="page-link" href="/search/">Search</a><a class="page-link" href="/capstone/">Capstone</a>
                    <a id="loginArea" class="page-link" href="/login">Login</a>
                </div>
            </nav></div>
    </header>

    <script type="module" src="/assets/js/api/login.js"></script>    


        

        

        <main class="page-content" aria-label="Content">
            <div class="wrapper">
                                <div class="opencs_root">
                                    












<style>
  /* === Post Header === */
  .post-header h3 {
    font-size: 1.8rem;
    font-weight: 600;
    margin-top: 0.5rem;
    margin-bottom: 0.5rem;
    line-height: 1.3;
  }

  .page-description {
    font-size: 1rem;
    color: #555;
    margin-bottom: 1rem;
  }

  /* === Meta Info (date, author, reading time) === */
  .post-meta {
    font-size: 0.9rem;
    color: #666;
    margin-bottom: 0.5rem;
  }

  .post-meta time {
    font-weight: 500;
  }

  /* === Category & Breadcrumb Links === */
  .category-tags-link {
    display: inline-block;
    padding: 0.2rem 0.6rem;
    margin: 0.1rem;
    font-size: 0.85rem;
    background: #f5f5f5;
    border-radius: 999px;
    color: #333;
    text-decoration: none;
    transition: background 0.2s ease;
  }

  .category-tags-link:hover {
    background: #e0e0e0;
  }

  .post-header {
    margin-bottom: 1rem;
  }

  .post-header-actions {
    margin-top: 0.85rem;
    display: flex;
    flex-wrap: wrap;
    gap: 0.45rem;
  }

  .post-primary-link {
    display: inline-flex;
    align-items: center;
    gap: 0.35rem;
    padding: 0.4rem 0.78rem;
    border: 1px solid #1d4ed8;
    border-radius: 999px;
    background: #2563eb;
    color: #ffffff;
    text-decoration: none;
    font-size: 0.83rem;
    font-weight: 700;
    line-height: 1.2;
    transition: background 0.2s ease, border-color 0.2s ease;
  }

  .post-primary-link:hover,
  .post-primary-link:focus-visible {
    background: #1d4ed8;
    border-color: #1e40af;
    color: #ffffff;
  }

  .post-secondary-link {
    display: inline-flex;
    align-items: center;
    gap: 0.35rem;
    padding: 0.35rem 0.7rem;
    border: 1px solid #d1d5db;
    border-radius: 999px;
    background: #f8fafc;
    color: #374151;
    text-decoration: none;
    font-size: 0.82rem;
    font-weight: 600;
    line-height: 1.2;
    transition: background 0.2s ease, border-color 0.2s ease, color 0.2s ease;
  }

  .post-secondary-link:hover,
  .post-secondary-link:focus-visible {
    background: #eef2f7;
    border-color: #9ca3af;
    color: #1f2937;
  }

  .post-header a.category-tags-link {
    margin-right: 0.3rem;
  }

  /* === Main Content Styling === */
  .post-content {
    line-height: 1.7;
    font-size: 1rem;
  }

  .post-content h2,
  .post-content h3 {
    margin-top: 1.5rem;
    margin-bottom: 0.75rem;
    border-bottom: 1px solid #eee;
    padding-bottom: 0.3rem;
  }

  /* === Comments Section Separator === */
  .post-content+div,
  .post-content+section {
    margin-top: 2rem;
    padding-top: 1rem;
    border-top: 1px solid #ddd;
  }

  /* Assignment Submission Widget */
  .assignment-submission {
    margin-top: 48px;
    padding: 24px;
    background: #f9f9f9;
    border: 1px solid #e0e0e0;
    border-radius: 12px;
  }

  .assignment-submission h3 {
    color: #333;
    font-size: 1.25rem;
    margin: 0 0 16px 0;
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .assignment-submission-icon {
    color: #2563eb;
  }

  .submission-options {
    display: flex;
    gap: 12px;
    margin-bottom: 20px;
    flex-wrap: wrap;
  }

  .submission-tab {
    padding: 8px 16px;
    background: white;
    border: 1px solid #d0d0d0;
    border-radius: 6px;
    color: #555;
    cursor: pointer;
    transition: all 0.2s;
  }

  .submission-tab:hover {
    background: #f0f0f0;
    color: #333;
  }

  .submission-tab.active {
    background: #2563eb;
    color: white;
    border-color: #2563eb;
  }

  .submission-form {
    display: none;
  }

  .submission-form.active {
    display: block;
  }

  .form-group {
    margin-bottom: 16px;
  }

  .form-group label {
    display: block;
    color: #333;
    font-size: 14px;
    margin-bottom: 8px;
    font-weight: 500;
  }

  .form-group input[type="text"],
  .form-group input[type="url"],
  .form-group textarea {
    width: 100%;
    padding: 10px 12px;
    background: white;
    border: 1px solid #d0d0d0;
    border-radius: 6px;
    color: #333;
    font-size: 14px;
    font-family: inherit;
  }

  .form-group input:focus,
  .form-group textarea:focus {
    outline: none;
    border-color: #2563eb;
  }

  .form-group textarea {
    min-height: 100px;
    resize: vertical;
  }

  .file-upload-area {
    border: 2px dashed #d0d0d0;
    border-radius: 8px;
    padding: 32px;
    text-align: center;
    cursor: pointer;
    transition: all 0.2s;
    background: white;
  }

  .file-upload-area:hover {
    border-color: #2563eb;
    background: #f0f7ff;
  }

  .file-upload-area.dragover {
    border-color: #2563eb;
    background: #f0f7ff;
  }

  .file-upload-icon {
    font-size: 48px;
    color: #2563eb;
    margin-bottom: 12px;
  }

  .file-upload-text {
    color: #555;
    margin-bottom: 8px;
  }

  .file-upload-hint {
    color: #999;
    font-size: 12px;
  }

  .file-list {
    margin-top: 16px;
  }

  .file-item {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 12px;
    background: white;
    border: 1px solid #e0e0e0;
    border-radius: 6px;
    margin-bottom: 8px;
  }

  .file-info {
    display: flex;
    align-items: center;
    gap: 12px;
  }

  .file-name {
    color: #333;
    font-size: 14px;
  }

  .file-size {
    color: #999;
    font-size: 12px;
  }

  .remove-file {
    background: transparent;
    border: none;
    color: #999;
    cursor: pointer;
    padding: 4px 8px;
    border-radius: 4px;
    transition: all 0.2s;
  }

  .remove-file:hover {
    background: #fee;
    color: #dc2626;
  }

  .submit-btn {
    padding: 12px 24px;
    background: #2563eb;
    color: white;
    border: none;
    border-radius: 6px;
    cursor: pointer;
    font-size: 14px;
    font-weight: 500;
    transition: all 0.2s;
    display: inline-flex;
    align-items: center;
    gap: 8px;
  }

  .submit-btn:hover {
    background: #1d4ed8;
  }

  .submit-btn:disabled {
    background: #d0d0d0;
    color: #999;
    cursor: not-allowed;
  }

  .submission-status {
    margin-top: 16px;
    padding: 12px;
    border-radius: 6px;
    display: none;
  }

  .submission-status.success {
    display: block;
    background: #dbeafe;
    border: 1px solid #2563eb;
    color: #1e40af;
  }

  .submission-status.error {
    display: block;
    background: #fee2e2;
    border: 1px solid #dc2626;
    color: #991b1b;
  }

  .submission-status.loading {
    display: block;
    background: #dbeafe;
    border: 1px solid #3b82f6;
    color: #1d4ed8;
  }
</style>

<article class="post h-entry" itemscope itemtype="http://schema.org/BlogPosting">

  <header class="post-header">
    
    Categories:
    <a class="category-tags-link" href="/search/#GitHub Pages">GitHub Pages</a>
    
    
    
    
    
    
    
    
    Breadcrumb:
    <a class="category-tags-link" href="/github/pages">/github/pages</a>
    
    
    
    <p class="post-meta post-meta-title"><time class="dt-published" datetime="2023-08-24T00:00:00+00:00" itemprop="datePublished">
        Aug 24, 2023
      </time>• <span class="read-time" title="Estimated read time">
    
     6 min read  </span></p>
    <h3>Anatomy of GitHub Pages</h3><p class="page-description">Learn the Files and development work flow of GitHub Pages.  This includes working with you home page, theme, markdown, and more.</p></header>

  <div class="post-content e-content" itemprop="articleBody"><ul><li>Anatomy of GitHub Pages files<ul><li>Files and Directories in this Project</li></ul></li><li>Configuration Notes, behind the scenes</li><li>Customizations<ul><li>Customize a Page</li><li>Change Title</li><li>Making a Submenu</li><li>Style revolves around _sass</li></ul></li></ul><div class="lesson-part" data-part="1" style="display:block;">

<h2>Anatomy of GitHub Pages files</h2>

<p>Discuss how to develop a home page, code, run local server test, and then sync to deploy to GitHub Pages.</p>

<p>Review tools setup and <code>make</code> in <code>README.md</code> to support this lesson.</p>

<h3>Files and Directories in this Project</h3>

<p>Here are some definitions to key files and directories in this project:</p>

<ul>
  <li><code>README.md</code>: This file contains instructions and background information about the project. It is a standard file present in all properly set up GitHub projects.</li>
  <li><code>index.md</code>: This is the source file for the home page of the project. It is a standard file for all GitHub Pages projects. Note that Markdown (.md) files are converted to HTML by the Jekyll build process. HTML files are the only file type that is rendered on a website.</li>
  <li><code>_notebooks</code>: This directory contains Jupyter Notebook (.ipynb) files. These files are converted to Markdown (.md) files by the Makefile rules in the build process. The Markdown files are then converted to HTML by the Jekyll build process.</li>
  <li><code>_posts</code>: This directory contains Markdown (.md) files that will be part of the website. These files are formatted similarly to index.md and include frontmatter (metadata coded in YAML) and Markdown, HTML, JavaScript, and CSS source code. You will also find Liquid code in these files, which is used to generate Markdown, HTML, JavaScript, and CSS.</li>
  <li><code>_data</code>: This directory is the standard location for storing data files that support the _posts or _notebooks directories.</li>
  <li><code>images</code>: This directory is the standard location for storing image files (JPEG, PNG, etc.) that support the _posts or _notebooks directories.</li>
  <li><code>_config.yml</code>: This file contains YAML definitions (key-value properties) used to build the Jekyll website.</li>
  <li><code>.gitignore</code>: This file specifies elements to be excluded from version control. Files are excluded when they are derived from the original source and not considered part of the project's source code. In the VSCode Explorer, you may notice some files appearing dimmed, indicating that they are purposely excluded by the rules in .gitignore.</li>
  <li><code>_layouts</code>: This directory contains HTML files used by Jekyll to generate the structure of the website, including blogs, schedules, and home pages. Each post or notebook specifies a layout in its frontmatter, which determines how the content is presented.</li>
  <li><code>scripts</code>: This directory contains scripts such as <code>convert_notebooks.py</code>, which converts Jupyter Notebook (.ipynb) files into Markdown (.md) files. These scripts automate parts of the build process, ensuring that content is properly formatted for the website.</li>
</ul>

<p>Please note that there are many other key files and directories in a GitHub Pages project, but we will highlight those as the development progresses.</p>

<div class="frq-box" data-frq-id="1" style="border:1px solid #ccc; padding:1rem; border-radius:8px; margin:1.5rem 0; box-sizing:border-box; overflow:auto; word-wrap:break-word; white-space:normal;">
    <b>FRQ 1:</b> What is the purpose of the <code>.gitignore</code> file and why is it important in a project's file structure?<br /><br />
    <textarea rows="5" placeholder="Type your response here..." style="width:100%; border-radius:6px; border:1px solid #ccc; padding:0.5rem; margin-top:0.5rem; box-sizing:border-box;"></textarea>
    <button class="grade-button" style="margin-top: 10px;">Grade</button>
    <div class="feedback-box"></div>
</div>
</div>
<hr />

<div class="lesson-part" data-part="2" style="display:none;">

<h2>Configuration Notes, behind the scenes</h2>

<p>The <code>_config.yml</code> file is the configuration file for Jekyll. It is a YAML file that defines the configuration of the site. The configuration file can be used to set site-wide variables, and can be used to set variables for specific environments (development, production, etc).</p>

<p>Often in code we use the <code>site.baseurl</code> to identify the path to files. GitHub actions uses this location in its build to identify the name of the project. Be sure the values of these keys match your GitHub Repo.</p>

<pre><code class="language-yaml">github_repo: "pages"
baseurl: "/pages"</code></pre>

<p>Many remote theme files are commented out, you can only have one at a time. The Teacher is in favor of using the <code>minima</code> theme. To change these themes it could require many other changes to make it effective. Themes and related CSS changes are below, but they are not complete. IMO, you would need to disable minima or reorganize a lot of files.</p>

<pre><code class="language-text">theme requirements
remote_theme: pages-themes/midnight@v0.2.0
remote_theme: pages-themes/dinky@v0.2.0
remote_theme: pages-themes/minimal@v0.2.0
remote_theme: pages-themes/hacker@v0.2.0
remote_theme: pages-themes/cayman@v0.2.0
remote_theme: pages-themes/time-machine@v0.2.0</code></pre>

<p>Under <code>_includes/theme</code> you will see directories that correspond to your selection. In each of these directories there is a <code>base.html</code>. This is the foundation for the page: head, body, footer. When you select a layout in the frontmatter of your pages, it ultimately includes the <code>base.html</code> from one of these directories. To understand how a web page is formed, these are excellent studies.</p>

<div class="frq-box" data-frq-id="2" style="border:1px solid #ccc; padding:1rem; border-radius:8px; margin:1.5rem 0; box-sizing:border-box; overflow:auto; word-wrap:break-word; white-space:normal;">
    <b>FRQ 2:</b> Describe the function of the <code>_config.yml</code> file in a Jekyll project. How does it relate to the <code>remote_theme</code> setting?<br /><br />
    <textarea rows="5" placeholder="Type your response here..." style="width:100%; border-radius:6px; border:1px solid #ccc; padding:0.5rem; margin-top:0.5rem; box-sizing:border-box;"></textarea>
    <button class="grade-button" style="margin-top: 10px;">Grade</button>
    <div class="feedback-box"></div>
</div>
</div>
<hr />

<div class="lesson-part" data-part="3" style="display:none;">

<h2>Customizations</h2>

<p>Each student should perform customization to their project. This is an opportunity to learn a few concepts from the 'teacher' repository and then customize your own page to your personal interests.</p>

<h3>Customize a Page</h3>

<p>The home page to other pages is a common first step in building a project. To start you will need to form your <code>index.md</code> in your project, which behind the scenes is generated into an <code>index.html</code> by the GitHub Pages build process.</p>

<h3>Change Title</h3>

<p>Every page should have a <code>title</code>. Here is a frontmatter sample. This uses the <code>_layouts/page.html</code> that reads the frontmatter title and places it at the top page.</p>

<pre><code class="language-yaml">layout: page
title: My Title</code></pre>

<p>If you look at the page layout you will see it includes base, or <code>base.html</code> according to the selected theme. This nesting is foundation of how GitHub Pages and Jekyll work.</p>

<p>Look at some of the layouts that form schedule, search, blogs, and each post. Between this structure and Jekyll you can automate almost any reconfiguration of the notebooks and posts.</p>

<div class="frq-box" data-frq-id="3" style="border:1px solid #ccc; padding:1rem; border-radius:8px; margin:1.5rem 0; box-sizing:border-box; overflow:auto; word-wrap:break-word; white-space:normal;">
    <b>FRQ 3:</b> What is the purpose of "frontmatter" in a Jekyll Markdown file, and how does the <code>layout</code> key specifically function?<br /><br />
    <textarea rows="5" placeholder="Type your response here..." style="width:100%; border-radius:6px; border:1px solid #ccc; padding:0.5rem; margin-top:0.5rem; box-sizing:border-box;"></textarea>
    <button class="grade-button" style="margin-top: 10px;">Grade</button>
    <div class="feedback-box"></div>
</div>
</div>
<hr />

<div class="lesson-part" data-part="4" style="display:none;">

<h3>Making a Submenu</h3>

<p>There are many submenus made in <code>_includes/nav</code>.</p>

<ul>
  <li><code>index.md</code> is the file that contains markdown for a submenu</li>
  <li><code></code> refers to baseurl defined in <code>_config.yml</code>, this is the location of all files in the Website. Note, this changes as you run on localhost and deployed; make sure you remember to use this for locations of files in site.</li>
</ul>

<pre><code class="language-html">&lt;table&gt;
&lt;tr&gt;
&lt;td&gt;&lt;img src="/images/logo.png" height="60" title="Frontend" alt=""&gt;&lt;/td&gt;
&lt;td&gt;&lt;a href="/index"&gt;Course&lt;/a&gt;&lt;/td&gt;
&lt;td&gt;&lt;a href="/home/table"&gt;Table&lt;/a&gt;&lt;/td&gt;
&lt;td&gt;&lt;a href="/home/about"&gt;About&lt;/a&gt;&lt;/td&gt;
&lt;/tr&gt;
&lt;/table&gt;</code></pre>

<p>Look how the same submenu is included on all of the pages it calls, you will notice this in the frontmatter menu key.</p>

<div class="frq-box" data-frq-id="4" style="border:1px solid #ccc; padding:1rem; border-radius:8px; margin:1.5rem 0; box-sizing:border-box; overflow:auto; word-wrap:break-word; white-space:normal;">
    <b>FRQ 4:</b> Explain the role of <code></code> in Jekyll. Why is it important to use this variable instead of a hardcoded path like <code>/images/logo.png</code>?<br /><br />
    <textarea rows="5" placeholder="Type your response here..." style="width:100%; border-radius:6px; border:1px solid #ccc; padding:0.5rem; margin-top:0.5rem; box-sizing:border-box;"></textarea>
    <button class="grade-button" style="margin-top: 10px;">Grade</button>
    <div class="feedback-box"></div>
</div>
</div>
<hr />

<div class="lesson-part" data-part="5" style="display:none;">

<h3>Style revolves around _sass</h3>

<p>In the <code>_sass</code> folder there are many theme files. Remember that our themes are <code>remote</code> as designated in the <code>_config.yml</code> line. However, some files are placed in the _sass directory to make customizations. It is best to only have files in your project that you need to customize.</p>

<p>The <code>_sass/minima</code> folder is a theme with many subthemes that can be changed in the <code>_sass/minima/custom-styles.scss</code> file. In the below example <code>_dracula</code>. You could switch to leaf, hacker, hamilton, etc. Then you will want to decide if you want <code>dark-mode</code>. Always include the <code>nighthawk/main</code> as it has customization to style for Nighthawk Pages.</p>

<pre><code class="language-scss">// Comment in or Uncomment out the following themes to use them
// Dark themes
//@import "minima/leaf/_leaf";  //Leaf theme
//@import "minima/hacker/jekyll-theme-hacker"; //Hacker theme
@import "minima/dracula/_dracula";
// Light themes
//@import "minima/hamilton/main"; //Hamilton theme
//@import "minima/monophase/main"; //Monophase theme
//@import "minima/minimal-mistakes/__minimal-mistakes"; //Minimal Mistakes theme
// Mix Light themes with this if your eyes are bleeding
@import "minima/dracula/dark-mode";
// Styles for nighthawk theme, do not remove
@import "nighthawk/main";</code></pre>

<div class="frq-box" data-frq-id="5" style="border:1px solid #ccc; padding:1rem; border-radius:8px; margin:1.5rem 0; box-sizing:border-box; overflow:auto; word-wrap:break-word; white-space:normal;">
    <b>FRQ 5:</b> Explain the purpose of the <code>@import</code> rule within an SCSS file like <code>custom-styles.scss</code>. How does this allow for theme customization?<br /><br />
    <textarea rows="5" placeholder="Type your response here..." style="width:100%; border-radius:6px; border:1px solid #ccc; padding:0.5rem; margin-top:0.5rem; box-sizing:border-box;"></textarea>
    <button class="grade-button" style="margin-top: 10px;">Grade</button>
    <div class="feedback-box"></div>
</div>
</div>

<script>
    const FRQ_QUESTIONS = {
        '1': "What is the purpose of the .gitignore file and why is it important in a project's file structure?",
        '2': "Describe the function of the _config.yml file in a Jekyll project. How does it relate to the remote_theme setting?",
        '3': "What is the purpose of frontmatter in a Jekyll Markdown file, and how does the layout key specifically function?",
        '4': "Explain the role of  in Jekyll. Why is it important to use this variable instead of a hardcoded path like /images/logo.png?",
        '5': "Explain the purpose of the @import rule within an SCSS file like custom-styles.scss. How does this allow for theme customization?"
    };
    const gradeButtons = document.querySelectorAll('.grade-button');
    gradeButtons.forEach(button => {
        button.addEventListener('click', async () => {
            const frqBox = button.closest('.frq-box');
            const frqId = frqBox.dataset.frqId;
            const questionText = FRQ_QUESTIONS[frqId];
            const studentResponseTextArea = frqBox.querySelector('textarea');
            const feedbackBox = frqBox.querySelector('.feedback-box');
            const studentResponse = studentResponseTextArea.value.trim();
            if (!studentResponse) {
                showModal("Please enter your response before submitting.");
                return;
            }
            // Show loading state
            button.disabled = true;
            feedbackBox.style.display = 'block';
            feedbackBox.innerHTML = '<div class="flex items-center space-x-2"><div class="loading-spinner"></div><span>Grading...</span></div>';
            try {
                const systemPrompt = `
                    You are an expert tutor grading a student's answer to a free-response question about Jekyll and Liquid.
                    Your task is to:
                    1. Determine a grade for the student's response based on the following 1-5 scale:
                        - 5: The answer addresses all parts of the question and is detailed and comprehensive.
                        - 4: The answer is correct and addresses most parts of the question.
                        - 3: The answer is correct but may be incomplete or lack detail.
                        - 2: The answer has significant inaccuracies or is incomplete.
                        - 1: The answer is incorrect or does not address the question.
                        Write the grade like this: "Grade: (1-5)/5"
                    2. Provide detailed, constructive feedback explaining the grade.
                    3. Offer very short suggestions on what the user could improve on, enough to give them a hint but not enough for them to figure out what to answer.
                    The question is: "${questionText}"
                    The student's response is: "${studentResponse}"
                    Format your final output with a clear heading for the grade and the feedback. Also, in the final output don't include hashtags to make your text bigger, it messes with the system on my end.
                `;
                const apiKey = "AIzaSyA3-LeTIUkZcYpb_DNZhrzgb5NJtE8bewc";
                const apiUrl = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-05-20:generateContent?key=${apiKey}`;
                const payload = {
                    contents: [{
                        parts: [
                            { text: systemPrompt }
                        ]
                    }]
                };
                const response = await fetchWithBackoff(apiUrl, {
                    method: 'POST',
                    headers: { 'Content-Type': 'application/json' },
                    body: JSON.stringify(payload)
                });
                if (!response.ok) {
                    throw new Error(`HTTP error! status: ${response.status}`);
                }
                const result = await response.json();
                const feedbackText = result?.candidates?.[0]?.content?.parts?.[0]?.text || "Could not generate feedback. Please try again.";
                const formattedFeedback = feedbackText
                    .replace(/\*\*(.*?)\*\*/g, '<strong>$1</strong>')
                    .replace(/\n/g, '<br>');
                feedbackBox.innerHTML = formattedFeedback;
                // Unlock next part if grade is 4 or 5
                const gradeMatch = feedbackText.match(/Grade:\s*(\d)\/5/);
                if (gradeMatch && parseInt(gradeMatch[1], 10) >= 4) {
                    const currentPart = parseInt(frqBox.closest('.lesson-part').dataset.part, 10);
                    const nextPart = document.querySelector(`.lesson-part[data-part="${currentPart + 1}"]`);
                    if (nextPart) {
                        nextPart.style.display = 'block';
                        nextPart.scrollIntoView({ behavior: 'smooth' });
                    }
                }
            } catch (error) {
                console.error("Error generating feedback:", error);
                feedbackBox.innerHTML = `<span style="color:red;">An error occurred while grading. Please try again.</span>`;
            } finally {
                button.disabled = false;
            }
        });
    });
    // Auto-save FRQ responses into localStorage
    document.addEventListener("DOMContentLoaded", () => {
        document.querySelectorAll(".frq-box textarea").forEach((textarea, index) => {
            const key = "jekyll_frq_answer_" + index;
            const saved = localStorage.getItem(key);
            if (saved) {
                textarea.value = saved;
            }
            textarea.addEventListener("input", () => {
                localStorage.setItem(key, textarea.value);
            });
        });
    });
    // Simple modal for alerts
    function showModal(message) {
        const modal = document.createElement('div');
        modal.className = 'modal';
        modal.innerHTML = `
            <div class="modal-content">
                <p>${message}</p>
                <button class="modal-button" onclick="this.closest('.modal').remove()">OK</button>
            </div>
        `;
        document.body.appendChild(modal);
    }
    // Exponential backoff for API retries
    async function fetchWithBackoff(url, options, retries = 3, delay = 1000) {
        for (let i = 0; i < retries; i++) {
            try {
                const response = await fetch(url, options);
                if (response.status === 429 && i < retries - 1) {
                    await new Promise(res => setTimeout(res, delay));
                    delay *= 2;
                    continue;
                }
                return response;
            } catch (error) {
                if (i < retries - 1) {
                    await new Promise(res => setTimeout(res, delay));
                    delay *= 2;
                    continue;
                }
                throw error;
            }
        }
    }
</script>



    

    

    
  </div><!-- from https://github.com/utterance/utterances -->
<script src="https://utteranc.es/client.js"
        repo="open-coding-society/pages"
        issue-term="title"
        label="blogpost-comment"
        theme="github-light"
        crossorigin="anonymous"
        async>
</script><a class="u-url" href="/github/pages/anatomy" hidden></a>

  <!-- Enhanced Analytics Tracking -->
  <script type="module">
    import { pythonURI, javaURI, fetchOptions } from '/assets/js/api/config.js';
    window.pythonURI = pythonURI;
    window.javaURI = javaURI;
    window.fetchOptions = fetchOptions;
  </script>
  <script src="/assets/js/ocs-analytics-enhanced.js"></script>
  <script src="/assets/js/code-runner-analytics.js"></script>
  <script src="/assets/js/lesson-completion.js"></script>
  <script src="/assets/js/lesson-completion-bigsix.js"></script>
</article>


                                </div>
            </div>
        </main><footer id="masterFooter" class="site-footer h-card">
    <data class="u-url" href="/"></data>

    <!-- <div class="wrapper">

        <div class="social-links"><ul class="social-media-list"><li>
    <a rel="me" href="" target="_blank" title="">
      <span class="grey fa-brands fa- fa-lg"></span>
    </a>
  </li><li>
    <a rel="me" href="" target="_blank" title="">
      <span class="grey fa-brands fa- fa-lg"></span>
    </a>
  </li><li>
    <a rel="me" href="" target="_blank" title="">
      <span class="grey fa-brands fa- fa-lg"></span>
    </a>
  </li>
  <li>
    <a href="/feed.xml" target="_blank" title="Subscribe to syndication feed">
      <svg class="svg-icon grey" viewbox="0 0 16 16">
        <path d="M12.8 16C12.8 8.978 7.022 3.2 0 3.2V0c8.777 0 16 7.223 16 16h-3.2zM2.194
          11.61c1.21 0 2.195.985 2.195 2.196 0 1.21-.99 2.194-2.2 2.194C.98 16 0 15.017 0
          13.806c0-1.21.983-2.195 2.194-2.195zM10.606
          16h-3.11c0-4.113-3.383-7.497-7.496-7.497v-3.11c5.818 0 10.606 4.79 10.606 10.607z"
        />
      </svg>
    </a>
  </li>
</ul>
</div>

    </div> -->

    <!--<p style="font-style: italic;">OpenAesthetic v3.0rc1.1</p>-->

    <div class="footer-links">
        <div class="footer-previous">
            
        </div>

        <div class="footer-home">
            
        </div>

        <div class="footer-next">
            
        </div>
    </div>

</footer>
<script src="https://cdn.jsdelivr.net/npm/mermaid@10/dist/mermaid.min.js"></script>
<script>
    document.addEventListener('DOMContentLoaded', function() {
        const style = getComputedStyle(document.documentElement);
        const theme = style.getPropertyValue('--theme').trim() || "dark";
        const panel = style.getPropertyValue('--panel-mid').trim() || "#0b1220";
        const text = style.getPropertyValue('--pref-text-color').trim() || "#e6eef8";
        const accent = style.getPropertyValue('--pref-accent-color').trim() || "#3b82f6";
        const fontFamily = style.getPropertyValue('--pref-font-family').trim() || "Arial, sans-serif";
        mermaid.initialize({ 
            startOnLoad: false,
            theme: theme,
            securityLevel: 'loose',
            themeVariables: {
                background: panel,
                primaryColor: panel,
                primaryTextColor: text,
                primaryBorderColor: accent,
                lineColor: text,
                arrowheadColor: text,
                fontFamily: fontFamily
            }
        });
        
        // Convert fenced code blocks to mermaid divs
        document.querySelectorAll('pre code.language-mermaid').forEach((block, index) => {
            const content = block.textContent;
            const wrapper = document.createElement('div');
            wrapper.className = 'mermaid';
            wrapper.id = 'mermaid-' + index;
            wrapper.textContent = content;
            block.parentElement.parentNode.replaceChild(wrapper, block.parentElement);
        });
        
        mermaid.run();
    });
</script></body>
</html>