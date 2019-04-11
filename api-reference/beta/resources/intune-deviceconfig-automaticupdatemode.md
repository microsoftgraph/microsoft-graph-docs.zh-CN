---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9af00bda442c1a152820323fc0b7e1ddfcd8c384
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791479"
---
# <a name="automaticupdatemode-enum-type"></a>automaticUpdateMode 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

自动更新模式的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|用户定义, 默认值, 无意向。|
|notifyDownload|1|下载时通知。|
|autoInstallAtMaintenanceTime|双面|在维护时间自动安装。|
|autoInstallAndRebootAtMaintenanceTime|第三章|在维护时间自动安装和重启。|
|autoInstallAndRebootAtScheduledTime|4|在计划的时间自动安装和重启。|
|autoInstallAndRebootWithoutEndUserControl|5|在没有最终用户控件的情况下自动安装和重启|
|windowsDefault|型|重置为 Windows 默认值。|





