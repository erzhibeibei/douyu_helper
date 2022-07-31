
请各位使用 Actions 时务必遵守Github条款。不要滥用Actions服务。

[日志示例](https://github.com/TheSlientnight/douyu_helper/runs/2078519193?check_suite_focus=true)

### 二、本地执行(不推荐)

#### Windows命令行内执行
执行步骤类似于GitHub执行，但是需要将你的COOKIE放入到系统的环境变量中
1. 将代码clone到本地或直接下载压缩包
2. 添加环境变量
   
    ![](docs/img/Path1.png)
    ![](docs/img/Path2.png)
    ![](docs/img/Path3.jpg)
   
3. 修改config.ini,详细做法可见[修改config配置](#一、Actions方式(推荐))
4. 进入项目根目录，使用指令
```shell
python main.py
```

#### Linux命令行执行
执行步骤同Windows执行，但是环境变量需要配置到/etc/Profile中
![](docs/img/Linux1.png)
![](docs/img/Linux2.png)
添加完成后需要重新读取，使用指令
```shell
source /etc/profile
```
### 三、Docker镜像
* [ ] 待更新

### 四、版本记录
V1.0 工具开源

V1.1 修复平均分配问题
