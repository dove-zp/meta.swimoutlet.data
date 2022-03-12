# META
## Scraped product data for swimoutlet[dot]com

I couldn't find a good webscraper for ripping content to create a dataset for a project involving fashion and models. Ripping with [my other nsfw project (wsnx)](https://github.com/dove-zp/package.wsnx) ended up being to risky, so I decided to create my own tool to collect data at the source. This repository contains data collections that I've personally scraped and organized. 

## Branches


* [media](https://github.com/dove-zp/meta.swimoutlet.data/tree/media)
```sql
-- about: table `products` contains the columns: (id, title, type, url, meta, thumbnail, hd_images, sd_images, ld_images, hd_video, sd_video)
-- example: a query for obtaining `hd_video` files for products that contain the case insensitive word `bikini` 
SELECT hd_video FROM products WHERE (title LIKE "%bikini%" OR type LIKE "%bikini%") AND (hd_video IS NOT NULL AND hd_video != "")
```
* [prices](https://github.com/dove-zp/meta.swimoutlet.data/tree/prices)
```sql
-- todo...
```

<!--  -->

## Feedback

I welcome your constructive input - both negative and positive. I will continue to try to provide updates when able. At some point you may find errors, inconsistencies, or methods that could be improved, or are missing altogether. Your feedback is critical to help improve future revisions.

The best way to reach out is by opening a new issue in this repository:

https://github.com/dove-zp/meta.swimoutlet.data/issues

Please be sure to refer to what your situation is when giving feedback and if possible link the topic in question.

Many thanks.

<hr/>

<p align="center">
  <p align="center">
    <a href="https://hits.seeyoufarm.com/api/count/graph/dailyhits.svg?url=https://github.com/dove-zp/meta.swimoutlet.data">
      <img src="https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fdove-zp%2Fmeta.swimoutlet.data&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=true" alt="repository hits">
    </a>
    <a href="https://github.com/dove-zp/meta.swimoutlet.data/releases">
      <img src="https://img.shields.io/github/downloads/dove-zp/meta.swimoutlet.data/total?style=flat-square" alt="downloads"/>
    </a>
    <a href="https://github.com/dove-zp/meta.swimoutlet.data/graphs/contributors">
      <img src="https://img.shields.io/github/contributors/dove-zp/meta.swimoutlet.data?style=flat-square" alt="contributors"/>
    </a>
    <a href="https://github.com/dove-zp/meta.swimoutlet.data/watchers">
      <img src="https://img.shields.io/github/watchers/dove-zp/meta.swimoutlet.data?style=flat-square" alt="watchers"/>
    </a>
    <a href="https://github.com/dove-zp/meta.swimoutlet.data/stargazers">
      <img src="https://img.shields.io/github/stars/dove-zp/meta.swimoutlet.data?style=flat-square" alt="stars"/>
    </a>
    <a href="https://github.com/dove-zp/meta.swimoutlet.data/network/members">
      <img src="https://img.shields.io/github/forks/dove-zp/meta.swimoutlet.data?style=flat-square" alt="forks"/>
    </a>
  </p>
</p>

<p align="center">
  <a href="https://github.com/dove-zp">
    <img width="64" heigth="64" src="https://avatars.githubusercontent.com/u/89095890" alt="dove-zp"/>
  </a>  
</p>
