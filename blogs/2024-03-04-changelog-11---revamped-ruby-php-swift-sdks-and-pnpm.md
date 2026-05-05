---
title: "Changelog #11 - Revamped Ruby, PHP, Swift SDKs and pnpm"
url: "https://konfigthis.com/blog/changelog-11"
date: "Mon, 04 Mar 2024 00:00:00 GMT"
author: ""
feed_url: "https://konfigthis.com/blog/rss.xml"
---
<p><img alt="banner" class="img_ev3q" height="819" src="https://konfigthis.com/assets/images/banner-c93e621352a0a318cab7b8c516b50c59.png" width="1560" /></p>
<p>In this changelog, we're excited to announce the release of the revamped Ruby,
PHP, and Swift SDKs. We've also made a change to the TypeScript SDKs to use
<code>pnpm</code> instead of <code>yarn</code> or <code>npm</code>. This change has improved the reliability and
performance of our TypeScript SDKs.</p>
<p>Furthermore, we've made several improvements and fixes to the Konfig's SDKs.
These include various bug fixes, better documentation, security vulnerability
fixes, and more rigorous testing for PHP, Python, Ruby, Go, TypeScript, and
Swift SDKs.</p>
<h2 class="anchor anchorWithStickyNavbar_LWe7" id="revamped-ruby-php-and-swift-sdks">Revamped Ruby, PHP, and Swift SDKs<a class="hash-link" href="https://konfigthis.com/blog/changelog-11#revamped-ruby-php-and-swift-sdks" title="Direct link to Revamped Ruby, PHP, and Swift SDKs">​</a></h2>
<p><img alt="Revamped SDKs" class="img_ev3q" height="819" src="https://konfigthis.com/assets/images/revamped-sdks-3791dfe6dcbd966df7267ae08354b008.png" width="1560" /></p>
<p>We revamped the Ruby, PHP, and Swift SDKs to be more consistent with the
quality of our Python and TypeScript SDKs.  This includes:</p>
<ul>
<li>Improved code quality</li>
<li>Better test coverage</li>
<li>Better documentation</li>
</ul>
<p>In particular, we removed the array of <code>.md</code> files that were generated as
documentation and replaced it with the singular <code>README.md</code> file that includes
everything you need to know about the SDK. Putting everything on one page makes
it easier to navigate and find what you need.</p>
<figure class="mb-4"><div class="mb-2"><img alt="Improved README" class="mx-auto img_ev3q" height="1664" src="https://konfigthis.com/assets/images/readme-5689ac23ef84237b9a5dc9fc00459c63.png" width="2030" /></div><b><figcaption class="text-center font-light text-sm"><p><b>README.md</b> now includes a branded header, getting started instructions, and a reference section with documentation for every operation in the SDK. This screenshot was taken from <a href="https://github.com/passiv/snaptrade-sdks/tree/master/sdks/typescript#readme" rel="noopener noreferrer" target="_blank">SnapTrade's TypeScript SDK</a> which served as a template for all revamped SDKs.</p></figcaption></b></figure>
<h2 class="anchor anchorWithStickyNavbar_LWe7" id="konfigs-typescript-sdks-now-use-pnpm">Konfig's TypeScript SDKs now use <code>pnpm</code><a class="hash-link" href="https://konfigthis.com/blog/changelog-11#konfigs-typescript-sdks-now-use-pnpm" title="Direct link to konfigs-typescript-sdks-now-use-pnpm">​</a></h2>
<p><img alt="pnpm" class="img_ev3q" height="819" src="https://konfigthis.com/assets/images/pnpm-85f7e5ccd6ddc10f9fa215b1cf5fbe10.png" width="1560" /></p>
<p>Based on internal quality assurance and integration tests that we regularly run
on our SDKs, we found that <code>pnpm</code> is a better fit for our TypeScript SDKs.
It's faster, more reliable, and uses less disk space than <code>npm</code> or <code>yarn</code>.  The
breaking point for us was concurrency bugs that were not fixable while using
<code>yarn</code>. When switching to <code>pnpm</code>, we found that these issues were resolved
without special configuration. This change allowed us to fix flaky tests and
continually ensure our generator was working as expected.</p>
<!-- -->
<details class="details_lb9f alert alert--info details_b_Ee">Improvements and Fixes<div><div class="collapsibleContent_i85q"><ul>
<li>Fix lost descriptions when using <code>allOf</code> with a single schema</li>
<li>Fix bug where TypeScript SDK would send extra data in the request body</li>
<li>Add <code>"strict": true</code> to <code>tsconfig.json</code> in the generated TypeScript SDK</li>
<li>Fix OAuth 2.0 Token URL not being generated correctly in TypeScript SDK</li>
<li>Fix refreshing the token in the generated TypeScript SDK</li>
<li>Fix links in README.md not working on npmjs.com for the TypeScript SDK</li>
<li>Fix security vulnerability from <code>aiohttp</code> in the generated Python SDK</li>
<li>Add <code>x-konfig-prefix</code> support in Go, Ruby, PHP, Python, and TypeScript</li>
<li>Fix default naming logic for security requirements in Go, Ruby, PHP, Python, and TypeScript</li>
<li>Add more rigorous testing for the PHP SDK</li>
<li>Add more rigorous testing for the Python SDK</li>
<li>Add more rigorous testing for the Ruby SDK</li>
<li>Add more rigorous testing for the Go SDK</li>
<li>Add more rigorous testing for the TypeScript SDK</li>
<li>Add more rigorous testing for the Swift SDK</li>
<li>Add <code>securitySchemeOverride</code> to <code>konfig.yaml</code> to override security schemes</li>
<li>Cleanup interface of top-level client class C# SDK</li>
<li>Fix handling of upper-case "in" field in <code>securitySchemes</code> in the OpenAPI specification</li>
</ul></div></div></details>
