# vue-favicon
vue打包后favicon显示

vue打包后favicon显示不正常解决:
如果是http连接地址一般不会出错,
如果是用路径地址，一种可以配置的方式：
打包后文件被拷贝到static目录下，具体位置与原始路径有关，
所以把favicon.ico图片放在static(与src同级)下，
打包后图片在dist/static里，在
<link type="favicon" rel="shortcut icon" href="./static/favicon.ico" />
引入即可。
注：
favicon有缓存，排除掉问题后可以试试清缓存。
