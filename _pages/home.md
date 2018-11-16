---
ID: 24
post_title: Home
author: jeffpaul
post_excerpt: ""
layout: page
permalink: http://tidedocs.local/
published: true
post_date: 2018-11-16 01:45:51
---
<blockquote>A rising tide lifts all boats. -- United States President, John F. Kennedy (borrowed from the New England Council)</blockquote>
<h2>Vision</h2>
Inspired by the proverb <em>“A rising tide lifts all boats”</em>, when we lower the barrier of entry to writing and choosing quality code for enough people, it will lift the quality of code across the whole WordPress ecosystem. Tide’s vision is to make it easy to improve the quality of code throughout the WordPress ecosystem and help WordPress site owners make better choices about plugins and themes.
<h2>Overview</h2>
Tide is an automated tool to provide insight into WordPress code and highlight areas to improve the quality of plugins and themes.

Tide services are responsible for the following:
<ul>
 	<li>The <a href="/docs/sync/">Sync Server</a> polls the WordPress.org API's for themes and plugins to process and writes them to a queue.</li>
 	<li>The <a href="/docs/phpcs/">PHPCS Server</a> reads messages from a queue and runs reports against both plugins and themes, then sends the results back to the Tide API.</li>
 	<li>The <a href="/docs/lighthouse/">Lighthouse Server</a> reads messages from a queue and runs Google Lighthouse reports against the themes only, then sends the results back to the Tide API.</li>
</ul>
<h2>Architecture Diagram</h2>
The following diagram notes the Google Cloud Platform (GCP) components, Tide services components, and pending link with WordPress.org for the PHP Compatibility integration.

<img src="assets/images/architecture-diagram.png" alt="architecture diagram" />
<h2>Working with Tide</h2>
Tide is actively developed. Currently you can:
<ul>
 	<li><a href="search.md">search for plugins &amp; themes</a> on this site and see their audit reports</li>
 	<li><a href="/docs/prerequisites/">install Tide</a> locally</li>
 	<li>deploy Tide to <a href="/docs/gcp-prerequisites/">Google Cloud Platform</a></li>
</ul>
In the future you will be able to use Tide as a service - use it to test your plugins or themes during development.
<h2>Contributing</h2>
Please read our <a href="https://github.com/wptide/wptide/blob/develop/CONTRIBUTING.md">Contributing Guidelines</a> for details on our code of conduct and the process for submitting pull requests to us.
<h2>Contact Us</h2>
Have questions? Don't open an Issue, come join us in the <a href="https://wordpress.slack.com/messages/C7TK8FBUJ/"><code>#tide</code> channel</a> in <a href="https://make.wordpress.org/chat/">WordPress Slack</a>. Even though Slack is a chat service, sometimes it takes several hours for community members to respond — please be patient.