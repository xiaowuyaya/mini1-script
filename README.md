<!--
 * @Descripttion: 
 * @version: 
 * @Author: xiaowuyaya
 * @Date: 2021-11-16 17:20:53
-->
# mini1-script
zsw的迷你世界自动化脚本 
## 11月19日 update

> "version_name": "2.4.1",
> "version_code": "1",

#### 下载地址：[mini_QvQ_v2.4.1.apk](https://github.com/llw605/mini1-script/releases/download/untagged-e3d89cccf211e9ee2809/mini_QvQ_v2.4.1.apk)

1. 修复了再启动游戏时，因为waitFor()方法导致的阻塞bug(程序卡死)
2. 增加了判断main进程是否异常退出的模块，在程序应该进行时，如果main进程卡死，则重启，该模块每20秒检测一次
3. 修改了日志的输出格式
   
**TODO：checkEngines模块无法判断是否因为阻塞而导致的程序暂停，后续可以通过引擎之间通讯的方式解决，发送心跳包判断线程是否正常**



## 11月18日 update

> "version_name": "2.3.1",
> "version_code": "1",

#### 下载地址：（无）

1. 修改了版本更新的判断规则,
2. 修改了version.json的格式
3. ~~热更新模块~~（未使用，太多bug了）
4. *正在开发检测主程序异常重启功能（实验，未上线）（判断是否异常退出，未检测是否阻塞状态）*

**TODO 阻塞判断是否要做？ 代码中应该没有会阻塞的地方了。**

***


## 11月17日 update

> "version_name": "2.2.2",
> "version_code": "1",

#### 下载地址： [mini_QvQ_v2.2.2.apk](https://github.com/llw605/mini1-script/releases/download/app/mini_QvQ_v2.2.2.apk)

1. 添加了错误日志发送到邮件的功能,
2. 添加了检查更新的功能
3. 添加了关闭按钮
4. 修复了卡设置页的bug
5. 目录结构更新说明：
   
```
    -[FloatButton]        悬浮窗组件
    -[img]                图片资源
    -[libs]               依赖包
        --email.jar       邮件依赖
    -[main_dir]           主程序
        --func_work.js    方法库
        --img_res.js      图片资源隐射文件
        --operation.js    行为操作文件
    [res]                 更新资源路径
    -[util]               工具包
        --email.js        邮件模块
        --version.js      版本更新组件
    -float.js             悬浮窗程序(启动程序)
    -main.js              主程序入口
    -version.json         版本信息
```
**TODO: 检测主程序异常重启功能，热更新功能（是否对话框确定？）,自启动**

***

## 11月16日 update
> "version_name": "2.1.1",
> "version_code": "1",

1. 更新了悬浮窗的展示效果,
2. 添加了3个悬浮窗展开按钮：获取更新，开始运行/结束运行，相关信息"
3. 目录结构更新说明：
   
```
    -[FloatButton]        悬浮窗组件
    -[img]                图片资源
    -[main_dir]           主程序
        --func_work.js    方法库
        --img_res.js      图片资源隐射文件
        --operation.js    行为操作文件
    -float.js             悬浮窗程序(启动程序)
    -main.js              主程序入口
```

***

### 11月14日 init

> "version_name": "1.1.7",
> "version_code": "6",

1. 添加了悬浮窗启动应用的功能,
2. 完成了脚本功能的编写
3. 完善了相关日志记录
4. 目录结构： 
```
    -[img]                图片资源
    -func_work.js         方法库
    -img_res.js           图片资源隐射文件
    -operation.js         行为操作文件
    -uiWindow.js          悬浮窗程序(启动程序)
    -main.js              主程序入口
```