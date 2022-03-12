# META
## Scraped product data for swimoutlet[dot]com

I couldn't find a good webscraper for ripping content to create a dataset for a project involving fashion and models. Ripping with [my other `nsfw` project (wsnx)](https://github.com/dove-zp/package.wsnx) ended up being too risky, so I decided to create my own tool to collect data at the source. This repository contains data collections that I've personally scraped and organized. 

## Branches


* [media](https://github.com/dove-zp/meta.swimoutlet.data/tree/media)
```sql
-- about: table `products` contains the columns: (id, title, type, url, meta, thumbnail, hd_images, sd_images, ld_images, hd_video, sd_video)
-- entry sample: (6904648958120, 'Maaji The Sweetest Spot Crop Bikini Top', 'Bikinis', 'https://www.swimoutlet.com/products/maaji-the-sweetest-spot-crop-bikini-top-8138372', 'https://www.swimoutlet.com/products/maaji-the-sweetest-spot-crop-bikini-top-8138372.js;https://www.swimoutlet.com/products/maaji-the-sweetest-spot-crop-bikini-top-8138372.json;', 'https://cdn.shopify.com/s/files/1/0248/3024/6994/products/6904648958120-2t.jpg?v=1633447544', '//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904648958120-2t.jpg?v=1633447544;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-1a.jpg?v=1633447547;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-2a.jpg?v=1633447550;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-3a.jpg?v=1633447553;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-4a.jpg?v=1633447555;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-5a.jpg?v=1633447558;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-6a.jpg?v=1633447561;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi.jpg?v=1633447565;', '//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904648958120-2t_473x.jpg?v=1633447544;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-1a_473x.jpg?v=1633447547;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-2a_473x.jpg?v=1633447550;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-3a_473x.jpg?v=1633447553;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-4a_473x.jpg?v=1633447555;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-5a_473x.jpg?v=1633447558;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-6a_473x.jpg?v=1633447561;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi_473x.jpg?v=1633447565;', '//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904648958120-2t_160x.jpg?v=1633447544;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-1a_160x.jpg?v=1633447547;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-2a_160x.jpg?v=1633447550;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-3a_160x.jpg?v=1633447553;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-4a_160x.jpg?v=1633447555;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-5a_160x.jpg?v=1633447558;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi-6a_160x.jpg?v=1633447561;//cdn.shopify.com/s/files/1/0248/3024/6994/products/6904649220264-multi_160x.jpg?v=1633447565;', 'https://cdn.shopify.com/videos/c/vp/c52dc7c9a2aa4e3db98f63c0960df812/c52dc7c9a2aa4e3db98f63c0960df812.HD-720p-4.5Mbps.mp4', 'https://cdn.shopify.com/videos/c/vp/c52dc7c9a2aa4e3db98f63c0960df812/c52dc7c9a2aa4e3db98f63c0960df812.SD-480p-1.5Mbps.mp4')
-- query example: obtaining `hd_video` files for products that contain the case insensitive word `bikini` 
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
