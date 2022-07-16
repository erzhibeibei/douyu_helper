
   **Fork仓库之后，GitHub默认不自动执行Actions任务,请手动执行一次以检查工作流**
   ![运行任务](docs/img/Workfelow.png)
   
9. 如果需要修改每日执行任务的时间,请修改`.github/auto_donate_douyu.yaml`下的`schedule`
```y
  schedule:
    - cron: '00 1 * * *'
    # cron表达式，Actions时区是国际时间，国际时间1点的时候，国内时间是早上9点。
    # 示例： 每天晚上22点30执行 '30 14 * * *'
-   # 部分直播间会在周末开启双倍亲密度，可以修改时间表，实现每周末赠送
    # 示例： 每周天凌晨12点30分执行 '0 30 16 ? * 7 '
```
如果收到了 GitHub Action 的错误邮件，请检查 Cookies 是不是失效了，用户修改密码、踢除设备下线，会导致 COOKIES 失效

请各位使用 Actions 时务必遵守Github条款。不要滥用Actions服务。

Please be sure to abide by the Github terms when using Actions. Do not abuse the Actions service.

**查看Actions运行日志**
1. 进入Actions执行结果
    ![](docs/img/WatchAction.png)
2. 查看执行详情
    ![](docs/img/WatchAction2.png)
3. 查看执行日志
    ![](docs/img/WatchAction3.png)
   
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
