---
ID: 24
post_title: Home
author: jeffpaul
post_excerpt: ""
layout: page
permalink: http://tidedocs.local/home/
published: true
post_date: 2018-11-16 01:45:51
---
> A rising tide lifts all boats. -- United States President, John F. Kennedy (borrowed from the New England Council)

## Vision

Inspired by the proverb *“A rising tide lifts all boats”*, when we lower the barrier of entry to writing and choosing quality code for enough people, it will lift the quality of code across the whole WordPress ecosystem. Tide’s vision is to make it easy to improve the quality of code throughout the WordPress ecosystem and help WordPress site owners make better choices about plugins and themes.

## Overview

Tide is an automated tool to provide insight into WordPress code and highlight areas to improve the quality of plugins and themes.

Tide services are responsible for the following:

*   The [Sync Server][1] polls the WordPress.org API's for themes and plugins to process and writes them to a queue.
*   The [PHPCS Server][2] reads messages from a queue and runs reports against both plugins and themes, then sends the results back to the Tide API.
*   The [Lighthouse Server][3] reads messages from a queue and runs Google Lighthouse reports against the themes only, then sends the results back to the Tide API.

## Architecture Diagram

The following diagram notes the Google Cloud Platform (GCP) components, Tide services components, and pending link with WordPress.org for the PHP Compatibility integration.

![architecture diagram][4]

## Working with Tide

Tide is actively developed. Currently you can:

*   [search for plugins & themes][5] on this site and see their audit reports
*   [install Tide][6] locally
*   deploy Tide to [Google Cloud Platform][7]

In the future you will be able to use Tide as a service - use it to test your plugins or themes during development.

## Contributing

Please read our [Contributing Guidelines][8] for details on our code of conduct and the process for submitting pull requests to us.

## Contact Us

Have questions? Don't open an Issue, come join us in the [`#tide` channel][9] in [WordPress Slack][10]. Even though Slack is a chat service, sometimes it takes several hours for community members to respond — please be patient.

 [1]: /docs/sync/
 [2]: /docs/phpcs/
 [3]: /docs/lighthouse/
 [4]: assets/images/architecture-diagram.png
 [5]: search.md
 [6]: /docs/prerequisites/
 [7]: /docs/gcp-prerequisites/
 [8]: https://github.com/wptide/wptide/blob/develop/CONTRIBUTING.md
 [9]: https://wordpress.slack.com/messages/C7TK8FBUJ/
 [10]: https://make.wordpress.org/chat/