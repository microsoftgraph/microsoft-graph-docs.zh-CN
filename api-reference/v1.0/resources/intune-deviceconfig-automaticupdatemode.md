---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3a0cc2d3918573fca6480c6eecd07889534cda4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028572"
---
# <a name="automaticupdatemode-enum-type"></a>automaticUpdateMode 枚举类型

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



