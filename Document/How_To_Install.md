### How to install
In order to use susnote, environment with python3.x(higher than 3.4) is required.<br>
```
pip3 install -r requirements.txt
```
<br>
After python3 installed the all the requirements, postgres database is also required.<br>
[Install Postgres in Mac](https://www.postgresql.org/download/macosx/) <br>
[Install Postgres in Linux](https://www.postgresql.org/download/linux/ubuntu/) <br>
[Install postgres in Windows](https://www.postgresql.org/download/macosx/) <br>

Enter postgres-cli:<br>
    ```
    CREATE DATABASE susnote;
    ```<br>
Then use the command:<br>
    ```
    cd app
    python3 migration.py
    ```<br>
After all these work:<br>
    ```
    python3 server.py
    ```

### 如何安装
为了使用susnote, 需要安装python3.4以上的环境。
如果已经有这样的环境:<br>
    ```
    pip3 install -r requirements.txt
    ```
<br>
安装完环境之后，需要初始化数据库(postgres):<br>
[Mac系统](https://www.postgresql.org/download/macosx/) <br>
[Linux系统](https://www.postgresql.org/download/linux/ubuntu/) <br>
[Windows系统](https://www.postgresql.org/download/macosx/) <br>

安装完成后，进入到postgres-cli:<br>
    ```
    CREATE DATABASE susnote;
    ```
    <br>
然后:<br>
    ```
    cd app
    python3 migration.py
    ```
    <br>
最后通过以下命令启动服务:<br>
    ```
    python3 server.py
    ```
<br>
如果需要使用redis作为缓存。请在config文件中将redis的open选项设置为True，反之设置为False.(将使用本地缓存)

### Install through Docker:
