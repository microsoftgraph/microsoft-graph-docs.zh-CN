---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 58684517d3d6477b0647d29e28d1bd4e29dd1515
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732420"
---
# <a name="automaticupdatemode-enum-type"></a>automaticUpdateMode 枚举类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

自动更新模式的可能值。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|userDefined|0|用户定义，默认值，无意向。|
|notifyDownload|1|下载时通知。|
|autoInstallAtMaintenanceTime|2|在维护时自动安装。|
|autoInstallAndRebootAtMaintenanceTime|3|在维护时自动安装和重新启动。|
|autoInstallAndRebootAtScheduledTime|4|在计划的时间自动安装和重新启动。|
|autoInstallAndRebootWithoutEndUserControl|5|在没有最终用户控制的情况下自动安装和重新启动|





