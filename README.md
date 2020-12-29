# GeoServer_CN_FONTS
geoserver_cn_fonts，是一个封装好了常见的中文简繁字体的GeoServer docker镜像，Geoserver版本是2.17.4，参考了[oscarfonts/geoserver](https://hub.docker.com/r/oscarfonts/geoserver)。
# 特性
+ 开箱即用的CORS支持。
+ 开箱即用的中文字库，方便SLD配图。
+ 优化过的JVM选项。
+ 允许对geoserver 配置，插件等目录使用docker volumes挂载。
# 如何使用
```
docker run -d -p 8080:8080
-v ~/data_dir:/var/local/geoserver \
-v ~/exts_dir:/var/local/geoserver-exts \
-v ~/config_dir:/usr/local/tomcat/conf/Catelina/localhost \
zhangasyncjun/ geoserver_cnfonts:2.17.4 
```

