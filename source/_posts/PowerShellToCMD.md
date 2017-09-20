---
title: Win10系统将“此处打开PowerShell窗口”更改为“在此处打开命令窗口”
thumbnail: ''
comment: true
date: 2017-09-20 18:31:32
tags:
categories:
description:
---
从Windows 10开始，微软一直在推动的Windows PowerShell中的替代命令提示符。
一个这样的变化是Windows PowerShell是Win + X菜单中的默认条目，而不是命令提示符。此外，扩展右键菜单中的“打开命令窗口”也被“打开 PowerShell窗口”替换。
如果您希望通过Windows PowerShell 使用命令提示符，请使用以下注册表的修改将隐藏的扩展右键单击菜单中的“打开命令窗口”恢复。

1. 运行注册表编辑器（regedit）。

2. 导航到以下注册表项或通过在注册表编辑器的地址栏中输入

`Computer\HKEY_CLASSES_ROOT\Directory\Background\shell\Powershell\command`

3. 右击`command`，然后选择权限。在权限对话框中，单击或点击高级按钮。在“高级安全设置”对话框中，单击或点击“ 所有者”字段后的“ 更改”链接。当提示选择用户或组时，输入用户帐户的用户名（包括使用Microsoft帐户登录的电子邮件地址）在要选择的对象名称的文本字段中。

另一种方法是输入“管理员”组，将管理员组中的所有用户设置为所有者。
完成后，点击OK两次返回“权限”对话框。

在权限对话框中，选择管理员在顶部段组，然后检查复选框完全控制下允许在底部部分列。


完成后点击OK。

4. 右键单击右窗格中的HideBasedOnVelocityId值名称（其默认值数据为`0x00639bc8（6527944）`），然后选择重命名。将名称更改为`ShowBasedOnVelocityId`。

5. 此处“打开命令窗口”现在出现在扩展右键单击菜单中，当按住Shift +右键单击文件夹以及“此处打开PowerShell窗口”时。

如果您希望两者同时出现，您现在可以停止，并跳过其余的步骤。

6. 如果您只希望在此处打开“打开命令窗口”，并要删除PowerShell选项，请使用以下注册表项重复上述步骤`Computer\HKEY_CLASSES_ROOT\Directory\Background\shell\Powershell\command`


7. 右键单击右窗格中的ShowBasedOnVelocityId值名称（默认值数据为`0x00639bc8（6527944）`），然后选择重命名。将名称更改为`HideBasedOnVelocityId`。

8. 此处的“Open PowerShell窗口”现在已被删除，并在扩展右键单击菜单中禁用。

9. 要在扩展右键菜单中还原并显示或隐藏“命令提示符”窗口或PowerShell窗口，只需在`HideBasedOnVelocityId`或`ShowBasedOnVelocityId`的值之间切换即可。