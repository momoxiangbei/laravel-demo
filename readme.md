[laravel-demo具体教程](http://lvwenhan.com/laravel/398.html)
####插件安装及配置
1. 打开composer.json   "require": {"插件": "版本"}
2. 运行composer update 进行安装
3. 在app.config 中添加配置

####数据库的建立及迁移
1. 配置数据库的连接 app/config/database.php
2. 创建数据表 
    + php artisan migrate --package=cartalyst/sentry    
      sentry会在数据库中自动创建5张表
    + php artisan migrate:make create_articles_table --create=articles        
      在.app/database/migrations 下创建了数据库迁移文件        
      修改文件 用schema创建具体的表
    + php artisan migrate 数据库中的表就建好了
3. 

####models
1. 创建模型    
    + php artisan generate:model article  


####数据库填充
1. 创建数据库填充文件
    + php artisan generate:seed article           
      在app/database/seeds/下创建了一个填充文件
2. 更改填充文件
    + 使用Faker\Factory作为随机数据生成器
3. 配置DatabaseSeeder.php
    + 添加$this->call('ArticleTableSeeder');
4. 填充数据到数据库
    + php artisan db:seed

    














































