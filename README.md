# Dockerfile
## 分布式爬虫的部署环境,主要安装了scrapy,scrapy-redis等python包


## 部署

``` sh
docker pull ibbd/scrapy-redis  
docker run -d --name scrapy -v "$PWD":/var/www/crawler -w /var/www/crawler ibbd/scrapy-redis scrapy crawl poi -a priority=1 -a proceed=1 
```
