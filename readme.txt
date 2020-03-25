1. 通过 juypter notebook 使用

安装：
conda install jupyter notebook

https://blog.csdn.net/Qiang_brother/article/details/104071093
开启远程访问：
执行:
jupyter notebook --generate-config
生成配置文件
Writing default config to:  /home/ubuntu/.jupyter/jupyter_notebook_config.py 
修改配置
echo "c.NotebookApp.allow_remote_access = True" >>  /home/ubuntu/.jupyter/jupyter_notebook_config.py 

设置访问密码：
执行
jupyter notebook password
查看密码对应的密文：
/home/ubuntu/.jupyter/jupyter_notebook_config.json
将密文写入配置文件
/home/ubuntu/.jupyter/jupyter_notebook_config.py 
c.NotebookApp.password = u'sha1:8d...刚才生成密码时复制的密文'

启动：
nohup jupyter notebook &
tail -f nohup.out （查看url）

2. 通过 vscode 连接

3. 通过 ssh 连接

