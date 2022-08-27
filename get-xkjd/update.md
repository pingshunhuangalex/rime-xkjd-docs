---
description: 更新Rime、键道与码表
---

# 更新键道

用户应根据自己使用的操作系统自行选择相对应的Rime键道进行更新

{% tabs %}
{% tab title="Windows" %}
1. 右键单击屏幕右下角的Rime输入平台图标，并选择菜单中的`检查新版本`即可更新Rime

{% hint style="warning" %}
更新键道与码表会强制覆盖所有用户配置文件并将git远程仓库重新指向[键道官方仓库](https://github.com/xkinput/Rime\_JD)

有自定义配置文件（且使用`git`进行管理）的用户，请务必在执行以下更新步骤前先备份自己的配置目录`C:\Users\%USERNAME%\AppData\Roaming\Rime`
{% endhint %}

1. 双击运行`<安装工具解压目录>\start.bat`或是`<安装工具解压目录>\Rime_JD\Tools\SystemTools\WindowsTools\update.bat`来进行键道输入方案与码表的更新

{% hint style="info" %}
如果用户想在更新后恢复配置文件，请继续完成以下步骤（以下流程以“自定义配置优先于官方改动”为前提，且默认用户已使用`git`进行配置管理）
{% endhint %}

1. 右键单击屏幕右下角的Rime输入平台图标，并选择菜单中的`退出算法服务`
2. 将更新后的Rime文件夹所有内容`C:\Users\%USERNAME%\AppData\Roaming\Rime`（不包含git文件夹，因为更新后的`git`远程仓库已被重新指向[键道官方仓库](https://github.com/xkinput/Rime\_JD)）暂时备份于其它目录
3. 在确保Rime文件夹是清空的状态下（无隐藏`git`文件夹）将更新前备份的所有用户配置文件（包含`git`文件夹）还原到`C:\Users\%USERNAME%\AppData\Roaming\Rime`
4. 将暂时备份于其它目录的含官方改动的Rime文件夹内容（无隐藏`git`文件夹）合并覆盖到`C:\Users\%USERNAME%\AppData\Roaming\Rime`
5. 通过`git`查看审核官方改动的内容并解决其与用户配置间存在的任何冲突
6. 重新启动算法服务
7. 右键单击屏幕右下角的Rime输入平台图标，并选择菜单中的`重新部署`
8. 核实并测试后可将含有官方改动的配置文件推送至用户自己的配置仓库
9. 如用户已在Rime中设置备份目录，可在更新完成后右键单击屏幕右下角的Rime输入平台图标，并选择菜单中的`用户资料同步`进行备份
{% endtab %}

{% tab title="macOS" %}
1. 右键单击屏幕右上角的Rime输入平台图标，并选择菜单中的`检查新版本`即可更新Rime

{% hint style="warning" %}
更新键道与码表会强制覆盖所有用户配置文件并将git远程仓库重新指向[键道官方仓库](https://github.com/xkinput/Rime\_JD)

有自定义配置文件（且使用`git`进行管理）的用户，请务必在执行以下更新步骤前先备份自己的配置目录`Macintosh HD/Users/%USERNAME%/Library/Rime`
{% endhint %}

1.  运行仓库中的键道脚本文件来进行更新

    ```bash
    cd Rime_JD/Tools/SystemTools/MacTools/ && ./2update.sh
    ```

{% hint style="info" %}
如果用户想在更新后恢复配置文件，请继续完成以下步骤（以下流程以“自定义配置优先于官方改动”为前提，且默认用户已使用`git`进行配置管理）
{% endhint %}

1. 在macOS的`活动监视器`中退出`鼠须管（Squirrel）`
2. 将更新后的Rime文件夹所有内容`Macintosh HD/Users/%USERNAME%/Library/Rime`（不包含`git`文件夹，因为更新后的git远程仓库已被重新指向[键道官方仓库](https://github.com/xkinput/Rime\_JD)）暂时备份于其它目录
3. 在确保Rime文件夹是清空的状态下（无隐藏`git`文件夹）将更新前备份的所有用户配置文件（包含`git`文件夹）还原到`Macintosh HD/Users/%USERNAME%/Library/Rime`
4. 将暂时备份于其它目录的含官方改动的Rime文件夹内容（无隐藏`git`文件夹）合并覆盖到`Macintosh HD/Users/%USERNAME%/Library/Rime`
5. 通过`git`查看审核官方改动的内容并解决其与用户配置间存在的任何冲突
6. 再次切换至`鼠须管（Squirrel）`来重新启动算法服务
7. 右键单击屏幕右上角的Rime输入平台图标，并选择菜单中的`重新部署`
8. 核实并测试后可将含有官方改动的配置文件推送至用户自己的配置仓库
9. 如用户已在Rime中设置备份目录，可在更新完成后右键单击屏幕右上角的Rime输入平台图标，并选择菜单中的`用户资料同步`进行备份
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
