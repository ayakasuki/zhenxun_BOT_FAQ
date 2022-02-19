> 作者：卖桃翁恋歌/桃子
>
> 感谢[A_nmi](https://github.com/HibiKier)的更新 1.3现在运行还有很多插件被ignore，等A_nmi更新
>

```
 pip3 install poetry
 poetry install
```

1. 设置超级用户，打开 **.env.dev** 文件，在`SUPERUSERS`中添加自己的QQ

    ```
     SUPERUSERS=["123456789"]
    ```

    复制代码
2. 打开 **configs/config.py** 填写数据库数据

    ```
     # 数据库（必要）
     # 如果填写了bind就不需要再填写后面的字段了#）
     # 示例："bind": "postgresql://user:password@127.0.0.1:5432/database"
     bind: str = ""  # 数据库连接链接
     sql_name: str = "postgresql"
     user: str = ""  # 数据用户名
     password: str = ""  # 数据库密码
     address: str = ""  # 数据库地址
     port: str = ""  # 数据库端口
     database: str = ""  # 数据库名称

     ############################################################
     ### 如果你是与教程一模一样的命令代码，且数据库也在该服务器上 ###
     ############################################################
     # 可以直接复制以下配置
     bind: str = ""  # 数据库连接链接
     sql_name: str = "postgresql"
     user: str = "uname"
     password: str = "zhenxun"
     address: str = "127.0.0.1"
     port: str = "5432"
     database: str = "testdb"
    ```

    复制代码
3. 使用`python3 bot.py`启动真寻Bot，会在 **configs** 和 **data/configs** 目录下生成各种配置文件
4. 打开  **configs/config.yaml** ，里面包含的是各种插件的配置项，填写完毕后重启真寻Bot

　　打开 **/真寻目录**后 playwright 需要安装额外的系统环境，在命令行输入以下

```python
poetry shell
playweight install
```

　　  5.	更新从1.1.0 到 v1.3.0

> 记得备份**zhenxun/resources/img**与**zhenxun/data**目录,防止色图出错
>

　　  6.如果genshin下载资源出错

> 把**[链接下的py](https://github.com/HibiKier/zhenxun_bot/blob/main/plugins/genshin/query_resource_points/query_resource.py)**替换相应目录
>
> **zhenxun_bot/plugins/genshin/query_resource_points**
>
> ## **query_resource.py**
>

　　
