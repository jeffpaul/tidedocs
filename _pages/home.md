---
ID: 24
post_title: ""
author: jeffpaul
post_excerpt: ""
layout: page
permalink: http://tidedocs.local/
published: true
post_date: 2018-11-16 01:45:51
---
## Vision

> A rising tide lifts all boats. -- United States President, John F. Kennedy (borrowed from the New England Council)

Inspired by the proverb _“A rising tide lifts all boats”_, when we lower the barrier of entry to writing and choosing quality code for enough people, it will lift the quality of code across the whole WordPress ecosystem. Tide’s vision is to make it easy to improve the quality of code throughout the WordPress ecosystem and help WordPress site owners make better choices about plugins and themes.

## Overview

Tide is an automated tool to provide insight into WordPress code and highlight areas to improve the quality of plugins and themes.

Tide services are responsible for the following:

- The [Sync Server](/docs/sync/) polls the WordPress.org API's for themes and plugins to process and writes them to a queue.
- The [PHPCS Server](/docs/phpcs/) reads messages from a queue and runs reports against both plugins and themes, then sends the results back to the Tide API.
- The [Lighthouse Server](/docs/lighthouse/) reads messages from a queue and runs Google Lighthouse reports against the themes only, then sends the results back to the Tide API.

## Architecture Diagram

The following diagram notes the Google Cloud Platform (GCP) components, Tide services components, and pending link with WordPress.org for the PHP Compatibility integration.

![architecture diagram](http://tidedocs.local/wp-content/uploads/2018/11/architecture-diagram.png)

## Working with Tide

Tide is actively developed. Currently you can:

- [search for plugins & themes](search.md) on this site and see their audit reports
- [install Tide](/docs/prerequisites/) locally
- deploy Tide to [Google Cloud Platform](/docs/gcp-prerequisites/)

In the future you will be able to use Tide as a service - use it to test your plugins or themes during development.

## Contributing

Please read our [Contributing Guidelines](https://github.com/wptide/wptide/blob/develop/CONTRIBUTING.md) for details on our code of conduct and the process for submitting pull requests to us.

## Contact Us

Have questions? Don't open an Issue, come join us in the [`#tide` channel](https://wordpress.slack.com/messages/C7TK8FBUJ/) in [WordPress Slack](https://make.wordpress.org/chat/). Even though Slack is a chat service, sometimes it takes several hours for community members to respond — please be patient.