---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5d0723bef94d187452d6b622c290f7e4cb0182db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532619"
---
# <a name="automaticupdatemode-enum-type"></a>automaticUpdateMode 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

自动更新模式的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|定制|0|用户定义，默认值，无意向。|
|notifyDownload|1 |下载时通知。|
|autoInstallAtMaintenanceTime|2 |在维护时间自动安装。|
|autoInstallAndRebootAtMaintenanceTime|3 |在维护时间自动安装和重启。|
|autoInstallAndRebootAtScheduledTime|4 |在计划的时间自动安装和重启。|
|autoInstallAndRebootWithoutEndUserControl|5 |在没有最终用户控件的情况下自动安装和重启|




