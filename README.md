# 网站

## 安装 composer

网站：

[Composer (getcomposer.org)](https://getcomposer.org/)

测试：

composer -V

## 安装 laravel

更改镜像源：

composer config -g repo.packagist composer https://mirrors.aliyun.com/composer/

安装 laravel6

composer create-project --prefer-dist laravel/Laravel=6 [安装目录]

解决路由404问题：

* 方法一

  修改"phpstudy_pro/Extensions/Nginx1.15.11/conf/vhosts/[网站名称].conf"

  在 location 中加入:

  try_files $uri $uri/ /index.php?$query_string;

  ![01](https://github.com/Loser-dreamer/ET/blob/main/md-img/01.jpg)

* 方法二

  直接修改小皮

  ![02](https://github.com/Loser-dreamer/ET/blob/main/md-img/02.jpg)

