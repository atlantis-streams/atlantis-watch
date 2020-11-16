<img title="atlantis-watch" style="display: block; margin-left: auto; margin-right: auto; width: 50%;" src="https://atlantisstream.io/images/atlantis-logo.png">
<h1 align="center" style="font-size:60px;"> AtlantisWatch</h1>

<p align="center">
  <b>Records what you do</b> so that you can <i>monetize your data,</i> and know how you've spent your time</i>
</p>

<p align="center">

  <br>

  <b>
    <a href="https://atlantisstream.iot/">Website</a>
    — <a href="https://twitter.com/atlantisstream">Twitter</a>
    — <a href="https://t.me/atlantisstreams">Telegram</a>
    — <a href="https://github.com/ActivityWatch/activitywatch/releases">Discord</a>
  </b>
</p>


<details>
 <summary align="center" style="font-size:20px;">Table of Contents</summary>

 * [About](#about)
    * [Screenshots](#screenshots)
    * [Features](#features)
    * [Installation &amp; Usage](#installation--usage)
 * [About this repository](#about-this-repository)
    * [Server](#server)
    * [Watchers](#watchers)
    * [Libraries](#libraries)
 * [Contributing](#contributing)
 * [Questions](#questions)
</details>

## About
**AtlantisWatch is under active development.**

The goal of [AtlantisWatch](htttps://www.atlantisstream.io) is simple: *Enable the collection of as much valuable lifedata as possible without compromising user privacy.*

We've worked towards this goal by creating a application for safe storage of the data on the users local machine and as well as watchers which record data such as:

 - Currently active application and the title of its window
 - Currently active browser tab and it's title and URL
 - Keyboard and mouse activity, to detect if you are AFK ("away from keyboard") or not

It is up to you as user to collect as much as you want, or as little as you want (and we hope some of you will help write *watchers* so we can collect more).

AtlantisWatch was made possible by Erik Bjäreholt's [ActivityWatch](https://github.com/ActivityWatch/activitywatch).

### Screenshots

<span><img src="https://activitywatch.net/img/screenshot-v0.9.3-activity.png"   width="40%"></span>
<span><img src="https://activitywatch.net/img/screenshot-v0.8.0b9-timeline.png" width="40%"></span>


## Installation & Usage

Announcement coming soon, stay tuned on our social channels.

## Features

 - You own your data.
 - Data across your devices is synced.
 - Easy to get started.
 - High data resolution.
 - Open-source code.

## Repository

This repository is a bundle of the core components and official modules of AtlantisWatch, each managed as an individual `git submodule`. It's primary use is as a meta-package providing all the components in one repo; enabling easier packaging and installation. It is also where releases of the full suite are published (see [releases](https://github.com/ActivityWatch/activitywatch/releases)).

### Server

`aw-server` is the official implementation of the core service which the other AtlantisWatch services interact with. It provides a REST API to a datastore and query engine. It also serves the web interface developed in the `aw-webui` project (which provides the frontend part of the webapp).

The REST API includes:

 - Access to a datastore suitable for timeseries/timeperiod-data
 - A query engine and language for such data

The webapp includes:

 - Data visualization & browser
 - Query explorer
 - Export functionality 

### Watchers

AtlantisWatch comes pre-installed with two watchers, `aw-watcher-afk` which logs the presence/absence of user activity from keyboard and mouse input and `aw-watcher-window` which logs the currently active application and it's window title.

There are lots of other watchers for Atlantis Watch which can track more types of activity such as `aw-watcher-web` which tracks time spent on websites, multiple editor watchers which tracks spent time coding and many more! Coming soon, see our current list of watchers [here.](https://atlantisstream.io/watchers)

### Libraries

 - `aw-core` - core library, provides no runnable modules
 - `aw-client` - client library, useful when writing watchers

## Contributing

Want to help? Great! Check out the [CONTRIBUTING.md file](./CONTRIBUTING.md)!

## Questions

Have a question, suggestion, problem, or just want to say hi? Hit up our team on Twitter, Telegram, Discord, LinkedIn and Facebook, or send us an email to team@atlantisstream.io