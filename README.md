# daizhigev20
古代文献

关于检索：
1. 检索文字请直接在网页最上输入文字，在repository里面检索

2. 检索标题请:


<!DOCTYPE html>
<html>
<head>
  <link rel="search" type="application/opensearchdescription+xml" href="/opensearch.xml" title="GitHub:Help" />
  <title>
  
    
      Configuring a publishing source for GitHub Pages - User Documentation
    
  
  </title>
  
<link rel="icon" type="image/x-icon" href="/assets/images/site/favicon.ico">
<link rel="stylesheet" href="/assets/stylesheets/application.css">
<script src="/assets/javascripts/application.js"></script>

<meta name="Description" content=" You can configure GitHub Pages to publish your site's source files from master, gh-pages, or a /docs folder on your master branch for Project Pages and other Pages sites that meet certain criteria.  I…">

<script type="text/javascript">
  $(function() {
    $('#quicksearch-query').lunrSearch({
      
      indexUrl: '/search/search.json',
      
      quickSearchResults:  '.autocomplete-results',
      quickSearchEntries:  '.result-group',
      quickSearchTemplate: '#quicksearch-results-template',

      searchResults: '.search-container',
      searchEntries: '.search-results',
      searchTemplate: '#search-results-template'
    });
  });
</script>

<script type="text/javascript">

  var _gaq = _gaq || [];
  _gaq.push(['_setAccount', 'UA-3769691-27']);
  _gaq.push(['_trackPageview']);

  (function() {
    var ga = document.createElement('script'); ga.type = 'text/javascript'; ga.async = true;
    ga.src = ('https:' == document.location.protocol ? 'https://ssl' : 'http://www') + '.google-analytics.com/ga.js';
    var s = document.getElementsByTagName('script')[0]; s.parentNode.insertBefore(ga, s);
  })();

</script>
<meta http-equiv="Content-Type" content="text/html;charset=utf-8" />

</head>

<body id="com">

<div id="not-footer">
  


  <div id="header">
    <div class="clearfix">
      <h1 class="site-logo"><a href="/">GitHub Help</a></h1>

      <ul class="top-nav">
        
<li>
  <button class="js-dropdown-button dropdown-button">Version <div class="dropdown-caret"></div></button>
  <div class="dropdown-menu js-dropdown-menu">
    <a href="/">GitHub.com</a>
    
    <a href="/enterprise/2.15/">GitHub Enterprise 2.15</a>
    
    <a href="/enterprise/2.14/">GitHub Enterprise 2.14</a>
    
    <a href="/enterprise/2.13/">GitHub Enterprise 2.13</a>
    
    <a href="/enterprise/2.12/">GitHub Enterprise 2.12</a>
    
  </div>
</li>


        
          <li><a href="https://github.com/contact" onClick="_gaq.push(['_trackEvent', 'Contact Support', 'Configuring a publishing source for GitHub Pages', window.location.href]);">Contact Support</a></li>
<li><a href="https://github.com/">Return to GitHub</a></li>

        
      </ul>
    </div>
  </div>

  <div id="content-wrapper">

    <div class="site">
      


























      <div class="content-header small">
        <h6 class="breadcrumbs">
          
          <a href="/categories/github-pages-basics">GitHub Pages Basics</a>
          /
          
          Configuring a publishing source for GitHub Pages
        </h6>
        <div class="search-form small right">
          
  


<script id="quicksearch-results-template" type="text/mustache">
  <div class="header">
    <a class="initial quicksearch-seemore" href="/search?q=">See more results</a>
  </div>
  [[#entries]]
    <tr class="article">
      <td class="info">
        <a href="[[url]]" class="js-articles-quicksearch-link">[[title]]</a>
      </td>
    </tr>
  [[/entries]]
</script>

<form accept-charset="UTF-8" action="/search" id="articles-search" method="get"><div style="margin:0;padding:0;display:inline"><input name="utf8" type="hidden" value="&#x2713;" /></div>
  <div class="outer">
    <div class="inner fade-label">
      <input type="text" name="q" id="quicksearch-query" class="js-articles-quicksearch"
      placeholder="How can we help?" />
      <div class="search-form-btn">
        <button><span class="octicon octicon-search"></span></button>
      </div>
    </div>
  </div>
</form>
<div class="autocomplete-results" style="display: none;">
  <table class="result-group" border="0" cellpadding="0" cellspacing="0">
  </table>
</div>

        </div>
      </div>

      <div class="article js-hide-during-search">

        <h2>Configuring a publishing source for GitHub Pages</h2>

        <div id="article-platform-nav">
  <ul>
    <li class="platform-mac">
      <a href="#platform-mac" data-platform="mac">
        mac
      </a>
    </li>
    <li class="platform-windows">
      <a href="#platform-windows" data-platform="windows">
        windows
      </a>
    </li>
    <li class="platform-linux">
      <a href="#platform-linux" data-platform="linux">
        linux
      </a>
    </li>
    <li class="platform-all">
      <a href="#platform-all" data-platform="all">
        all
      </a>
    </li>
  </ul>
</div>


        <div class="article-body content-body wikistyle markdown-format">
          <div class='intro'>

          

          </div>

          <div class="intro">

<p>You can configure GitHub Pages to publish your site's source files from <code>master</code>, <code>gh-pages</code>, or a <code>/docs</code> folder on your <code>master</code> branch for Project Pages and other Pages sites that meet certain criteria.</p>

</div>

<p>If your site is a User or Organization Page that has a repository named 
<code>&lt;username&gt;.github.io</code>
 or 
<code>&lt;orgname&gt;.github.io</code>
, you cannot publish your site's source files from different locations. User and Organization Pages that have this type of repository name are only published from the <code>master</code> branch.</p>

<p>For more information about the different types of GitHub Pages sites, see "<a href="/articles/user-organization-and-project-pages">User, Organization, and Project Pages</a>."</p>

<h3>
<a id="default-source-settings-for-repositories-without-the-username-naming-scheme" class="anchor" href="#default-source-settings-for-repositories-without-the-username-naming-scheme" aria-hidden="true"><span aria-hidden="true" class="octicon octicon-link"></span></a>Default source settings for repositories without the username naming scheme</h3>

<p>The default settings for publishing your site's source files depend on your site type and the branches you have in your site repository.</p>

<p>If your site repository doesn't have a <code>master</code> or <code>gh-pages</code> branch, your GitHub Pages publishing source is set to <strong>None</strong> and your site is not published.</p>

<p><img src="/assets/images/help/pages/none-source-setting.png" alt="none-source-setting"></p>

<p>After you've created either a <code>master</code> or <code>gh-pages</code> branch, you can set one as your publishing source so that your site will be published.</p>

<p>If you fork or upload your site repository with only a <code>master</code> or <code>gh-pages</code> branch, your site's source setting will automatically be enabled for that branch.</p>

<h3>
<a id="enabling-github-pages-to-publish-your-site-from-master-or-gh-pages" class="anchor" href="#enabling-github-pages-to-publish-your-site-from-master-or-gh-pages" aria-hidden="true"><span aria-hidden="true" class="octicon octicon-link"></span></a>Enabling GitHub Pages to publish your site from <code>master</code> or <code>gh-pages</code>
</h3>

<p>To select <code>master</code> or <code>gh-pages</code> as your publishing source, you must have the branch present in your repository. If you don't have a <code>master</code> or <code>gh-pages</code> branch, you can create them and then return to source settings to change your publishing source.</p>

<ol>
<li>On GitHub, navigate to your GitHub Pages site's repository.</li>
<li><p>Under your repository name, click <span class="octicon octicon-gear" aria-label="The gear icon " title="The gear icon "></span>
<strong>Settings</strong>.
<img src="/assets/images/help/repository/repo-actions-settings.png" alt="Repository settings button"></p></li>
<li><p>Use the Select source drop-down menu to select <strong>master</strong> or <strong>gh-pages</strong> as your GitHub Pages publishing source.
<img src="/assets/images/help/pages/select-gh-pages-or-master-as-source.png" alt="select-gh-pages-or-master-as-source"></p></li>
<li>Click <strong>Save</strong>.
<img src="/assets/images/help/pages/click-save-next-to-source-selection.png" alt="click-save-next-to-source-selection">
</li>
</ol>

<h3>
<a id="publishing-your-github-pages-site-from-a-docs-folder-on-your-master-branch" class="anchor" href="#publishing-your-github-pages-site-from-a-docs-folder-on-your-master-branch" aria-hidden="true"><span aria-hidden="true" class="octicon octicon-link"></span></a>Publishing your GitHub Pages site from a <code>/docs</code> folder on your <code>master</code> branch</h3>

<p>To publish your site's source files from a <code>/docs</code> folder on your <code>master</code> branch, you must have a <code>master</code> branch and your repository must:</p>

<ul>
<li>have a <code>/docs</code> folder in the root of the repository</li>
<li>not follow the repository  naming scheme 
<code>&lt;username&gt;.github.io</code>
or 
<code>&lt;orgname&gt;.github.io</code>
</li>
</ul>

<p>GitHub Pages will read everything to publish your site, including the CNAME file, from the <code>/docs</code> folder. For example, when you edit your custom domain through the GitHub Pages settings, the custom domain will write to <code>/docs/CNAME</code>.</p>

<div class="alert tip">

<p><strong>Tip:</strong> If you remove the <code>/docs</code> folder from the <code>master</code> branch after it's enabled, your site won't build and you'll get a <a href="/articles/page-build-failed-missing-docs-folder">page build error message for a missing <code>/docs</code> folder</a>.</p>

</div>

<ol>
<li>On GitHub, navigate to your GitHub Pages site's repository.</li>
<li>Create a folder in the root of your repository on the <code>master</code> branch called <code>/docs</code>.</li>
<li><p>Under your repository name, click <span class="octicon octicon-gear" aria-label="The gear icon " title="The gear icon "></span>
<strong>Settings</strong>.
<img src="/assets/images/help/repository/repo-actions-settings.png" alt="Repository settings button"></p></li>
<li>
<p>Use the Select source drop-down menu to select <strong>master branch /docs folder</strong> as your GitHub Pages publishing source.
<img src="/assets/images/help/pages/select-master-branch-docs-folder-as-source.png" alt="select-master-branch-docs-folder-as-source"></p>

<div class="alert tip">

<p><strong>Tip:</strong> The <strong>master branch /docs folder</strong> source setting will not appear as an option if the <code>/docs</code> folder doesn't exist on the <code>master</code> branch.</p>

</div>
</li>
<li><p>Click <strong>Save</strong>.
<img src="/assets/images/help/pages/click-save-next-to-master-branch-docs-folder-source-selection.png" alt="click-save-next-to-master-branch-docs-folder-source-selection"></p></li>
</ol>

<h3>
<a id="further-reading" class="anchor" href="#further-reading" aria-hidden="true"><span aria-hidden="true" class="octicon octicon-link"></span></a>Further Reading</h3>

<ul>
<li><a href="/articles/viewing-branches-in-your-repository/">Viewing branches in your repository</a></li>
</ul>
        </div>

        <div class="support-footer">
  <ul class="article-footer button-nav">
    
      <li><a href="https://github.com/contact" class="minibutton" onClick="_gaq.push(['_trackEvent', 'Contact Support', 'Configuring a publishing source for GitHub Pages', window.location.href]);">
          <span class="octicon octicon-comment-discussion"></span>
          Contact a human
        </a>
      </li>
    
  </ul>
</div>

      </div>

      <div class="sidebar">
  <h3>Article versions</h3>
  <ul>
    <li><a href="#" skip-conversion data-proofer-ignore>GitHub.com</a></li>

    
      <li class="muted">
        <a data-proofer-ignore>GitHub Enterprise 2.15</a>
      </li>
    
      <li class="muted">
        <a data-proofer-ignore>GitHub Enterprise 2.14</a>
      </li>
    
      <li class="muted">
        <a data-proofer-ignore>GitHub Enterprise 2.13</a>
      </li>
    
      <li class="muted">
        <a data-proofer-ignore>GitHub Enterprise 2.12</a>
      </li>
    

  </ul>
</div>


      <div class="clear"></div>
    </div>
  </div>
</div>

<div id="footer">
  <div class="inner">
    <a href="https://github.com" class="invertocat">
      <img alt="The GitHub Logo" src="/assets/images/site/invertocat.png" width="24" height="24" />
    </a>
    <p class="left">
      &copy; <span id="year">2018</span> GitHub Inc. All rights reserved.
    </p>
      <ul class="links right">
        <li><a href="/terms-of-service">Terms of Service</a></li>
        <li><a href="/privacy-policy">Privacy</a></li>
        
          <li><a href="/security">Security</a></li>
        
        
          <li><a href="https://github.com/contact" onClick="_gaq.push(['_trackEvent', 'Contact Support', 'Configuring a publishing source for GitHub Pages', window.location.href]);">
              Support
            </a>
          </li>
        
      </ul>
  </div>
</div>


<div class="fullscreen-overlay"></div>
</body>
</html>
