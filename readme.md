[laravel-demo具体教程](http://lvwenhan.com/laravel/398.html)
####插件安装及配置
1. 打开composer.json   "require": {"插件": "版本"}
2. 运行composer update 进行安装
3. 在app.config 中添加配置

####数据库的建立及迁移
1. 配置数据库的连接 app/config/database.php
2. 创建数据库  
>php artisan migrate --package=cartalyst/sentry
3. 建立表

####models
1. 创建模型

####数据库填充


