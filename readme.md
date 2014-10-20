[laravel-demo具体教程](http://lvwenhan.com/laravel/398.html)
####插件安装及配置
1. 打开composer.json   "require": {"插件": "版本"}
2. 运行composer update 进行安装
3. 在app.config 中添加配置

####数据库的建立及迁移
1. 配置数据库的连接 app/config/database.php
2. 创建数据表 
    + php artisan migrate --package=cartalyst/sentry
    + sentry会在数据库中自动创建5张表
    + php artisan migrate:make create_articles_table --create=articles
    + 在.app/database/migrations 下创建了数据库迁移文件

3. 

####models
1. 创建模型

####数据库填充


