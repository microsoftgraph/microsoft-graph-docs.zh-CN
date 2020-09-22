---
title: userExperienceAnalyticsOperatingSystemRestartCategory 枚举类型
description: 操作系统重新启动类别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d78328cc9f44dbffca0085890a8c69184c2eac3b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48080801"
---
# <a name="userexperienceanalyticsoperatingsystemrestartcategory-enum-type"></a>userExperienceAnalyticsOperatingSystemRestartCategory 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

操作系统重新启动类别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知|
|restartWithUpdate|1 |重新启动并更新|
|restartWithoutUpdate|2 |重新启动而不更新|
|Options.bluescreen|第三章|蓝屏重启|
|shutdownWithUpdate|4 |使用更新进行关机|
|shutdownWithoutUpdate|5 |关闭而不更新|
|longPowerButtonPress|6 |长电源按钮按下|
|bootError|7 |启动错误|






