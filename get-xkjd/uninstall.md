---
description: 彻底移除键道及所有配置
---

# 卸载键道

用户应根据自己使用的操作系统自行选择相对应的Rime键道进行卸载

{% tabs %}
{% tab title="Windows" %}
1. 用户可前往`控制面板 → 程序 → 程序和功能`进行Rime卸载
2. 卸载完成后可通过删除`C:\Program Files (x86)\Rime`来清理冗余输入平台文件
3. 用户可前往安装键道时指定的解压目录来移除输入法安装工具
4. 用户可通过删除`C:\Users\%USERNAME%\AppData\Roaming\Rime`来彻底移除配置文件
5. 如仍不放心，用户可使用诸如`CCleaner`类的工具对注册表进行最后的清理
{% endtab %}

{% tab title="macOS" %}
1. 用户可前往`苹果图标 → 系统偏好设置 → 键盘 → 输入法 → 移除（-）按钮`来删除`鼠须管（Squirrel）`
2. 在macOS的`活动监视器`中退出`鼠须管（Squirrel）`
3. 用户可通过删除`Macintosh HD/Library/Input Methods/Squirrel.app`来卸载Rime
4. 用户可前往之前下载的键道仓库文件夹目录来移除输入法安装工具
5. 用户可通过删除`Macintosh HD/Users/%USERNAME%/Library/Rime`来彻底移除配置文件
6. 如仍不放心，用户可使用诸如`App Cleaner`类的工具对系统进行最后的清理
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
