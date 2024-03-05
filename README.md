# xhamster-scraper

A bash script for scraping xhamster videos,channels,creators,pornstars,galleries,users,posts metadata in json.

## Requirements

 - [hgrep](https://github.com/TUVIMEN/hgrep)
 - [jq](https://github.com/stedolan/jq)

## Installation

    install -m 755 xhamster-scraper /usr/bin

## Json format

Here's example of a [video](video-example.json), [pornstar](pornstar-example.json), [creator](creator-example.json), [channel](channel-example.json), [user](user-example.json), [gallery](gallery-example.json).

## Usage

Download metadata of videos to DIR

    xhamster-scraper DIR -v

Download metadata of pornstars to DIR

    xhamster-scraper DIR -p

Download metadata of creators to DIR

    xhamster-scraper DIR -c

Download metadata of channels to DIR

    xhamster-scraper DIR -C

Download metadata of galleries to DIR

    xhamster-scraper DIR -g

Download metadata of user to DIR from URL. Since users aren't in sitemap you have to compile list of users from previous results.

    xhamster-scraper DIR -u URL

Download users from links in FILE to DIR

    xhamster-scraper DIR -U FILE
