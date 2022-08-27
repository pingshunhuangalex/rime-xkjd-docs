---
description: 下载安装 + 恢复用户配置与主题预览
---

# 获取键道

用户应根据自己使用的操作系统自行选择相对应的Rime键道进行下载安装

{% tabs %}
{% tab title="Windows" %}
{% hint style="warning" %}
一般情况下，键道安装包中的脚本会自动下载最新版本的Rime

如果碰到脚本中的下载链接过期导致程序报错，用户可在执行键道安装程序前先自行前往[Rime官方仓库](https://github.com/rime/weasel/releases/latest)下载安装Rime**（须安装在默认路径下）**
{% endhint %}

1. 前往[键道官方仓库](https://github.com/xkinput/Rime\_JD)下载键道输入方案
2. 双击运行安装程序进行安装**（用户可自行选择解压路径，但应保证键道输入方案与Rime一同安装在默认路径下）**
3. 安装完成后如果Rime没有被自动添加到Windows输入法中，用户可前往`开始 → 设置 → 时间和语言 → 语言（中文）`进行添加
4. 安装完成后如果键道没有被自动添加到Rime输入平台中，用户可右键单击屏幕右下角的Rime输入平台图标，并选择菜单中的`输入法设定`，然后勾选「键道6」即可

> 安装如有疑惑，可同时参考[安装视频](https://www.bilibili.com/video/av53185153)

{% hint style="info" %}
如果用户想在安装后恢复配置或主题文件，请继续完成以下步骤
{% endhint %}

1. 右键单击屏幕右下角的Rime输入平台图标，并选择菜单中的`退出算法服务`
2. 将所有用户配置文件还原覆盖到`C:\Users\%USERNAME%\AppData\Roaming\Rime`
3. 将所有主题预览文件添加到`C:\Program Files (x86)\Rime\weasel-<版本号>\data\preview`
4. 重新启动算法服务
5. 右键单击屏幕右下角的Rime输入平台图标，并选择菜单中的`重新部署`
{% endtab %}

{% tab title="macOS" %}
1. 前往[Rime官方仓库](https://github.com/rime/squirrel/releases/latest)下载安装Rime**（须安装在默认路径下）**
2. 安装完成后如果Rime没有被自动添加到macOS输入法中，用户可前往`苹果图标 → 系统偏好设置 → 键盘 → 输入法 → 添加（+）按钮 → 简体中文 → 鼠须管（Squirrel）`进行添加
3.  下载[键道官方仓库](https://github.com/xkinput/Rime\_JD)**（用户可自行选择下载路径）**

    ```git
    git clone https://github.com/xkinput/Rime_JD/
    ```
4.  运行仓库中的键道脚本文件来进行安装

    ```bash
    cd Rime_JD/Tools/SystemTools/MacTools/ && ./2update.sh
    ```

{% hint style="info" %}
如果用户想在安装后恢复配置或主题文件，请继续完成以下步骤
{% endhint %}

1. 在macOS的`活动监视器`中退出`鼠须管（Squirrel）`
2. 将所有用户配置文件还原覆盖到`Macintosh HD/Users/%USERNAME%/Library/Rime`
3. 再次切换至`鼠须管（Squirrel）`来重新启动算法服务
4. 右键单击屏幕右上角的Rime输入平台图标，并选择菜单中的`重新部署`
{% endtab %}

{% tab title="Linux" %}
待验证补充，请先移步[键道官方仓库](https://github.com/xkinput/Rime\_JD)
{% endtab %}

{% tab title="Android" %}
待验证补充，请先移步[键道官方仓库](https://github.com/xkinput/Rime\_JD)
{% endtab %}

{% tab title="iOS" %}
待验证补充，请先移步[键道官方仓库](https://github.com/xkinput/Rime\_JD)
{% endtab %}
{% endtabs %}
