#我们怎样描述一个应用

## 从用户的视角：
应用名称
图标
封面（布局、slogan...）
页面格局
常规功能（登录、关于、帮助、反馈、分享...）

## 从应用商店的视角
应用名称
应用描述
作者
图标
平台（android/ios）
应用版本（{android:{versionName,versionCode}}, {iOS: {versionName, build}})
应用Id
签名
权限
截图
安装包体积
版本更新描述


## 从程序员的视角
工程名
工程目录
代码仓库（git/svn/gitflow）
开发工具/语言（flutter、react-native、weex）
第三方类库
适配的操作系统版本（{android: minSdkVersion,ios:i}）


OvO配置文件：用来描述你希望构建的App包含的特性。
OvO.yml

# 怎样根据描述创建应用框架
YAML是我们选择的计算机读的懂，人看着也不累的语言来记录配置文件。
YAML比json的优势在于，不必维护繁琐的"{}"嵌套问题。
你可以根据喜好，为你的应用选择配置文件文件名.
OvOFile
OvO.yaml
OvO.yml

## OvOFile 文件内容：

### 第一部分应用信息

AppInfo
|名称|Key|可选|默认|有效值|
|:---:|:---:|:---:|:---:|:---:|
|名称|AppName|必备||String|
|版本|Version|必备||String|
|图标|Logo|必备||fileName|

### 第二部分UI信息

UIInfo
|名称|Key|可选|默认|有效值|
|:---:|:---:|:---:|:---:|:---:|
|封面|Cover|可选|defaultCover|fileName|
|布局|Layout|可选|defaultLayout|Object|


### 第三部分工程信息
ProjectInfo
|名称|Key|可选|默认|有效值|
|:---:|:---:|:---:|:---:|:---:|
|工程名|ProjectName|必备||String|
|开发工具|Framework|必备||"ReactNative"\|"Flutter"|

