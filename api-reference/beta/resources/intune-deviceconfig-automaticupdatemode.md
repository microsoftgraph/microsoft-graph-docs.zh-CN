---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 845fdacfb0b29449e4464ec0eea03924632e861b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795903"
---
# <a name="automaticupdatemode-enum-type"></a>automaticUpdateMode 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

自动更新模式的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|用户定义，默认值，无意向。|
|notifyDownload|1|下载时通知。|
|autoInstallAtMaintenanceTime|双面|在维护时间自动安装。|
|autoInstallAndRebootAtMaintenanceTime|第三章|在维护时间自动安装和重启。|
|autoInstallAndRebootAtScheduledTime|4 |在计划的时间自动安装和重启。|
|autoInstallAndRebootWithoutEndUserControl|5 |在没有最终用户控件的情况下自动安装和重启|
|windowsDefault|6 |重置为 Windows 默认值。|



