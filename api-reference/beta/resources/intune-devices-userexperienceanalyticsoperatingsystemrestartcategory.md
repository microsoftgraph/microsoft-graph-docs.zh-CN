---
title: userExperienceAnalyticsOperatingSystemRestartCategory 枚举类型
description: 操作系统重启类别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8b68f119a463ad2e2cae5f5907e54188814f7ed3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58783209"
---
# <a name="userexperienceanalyticsoperatingsystemrestartcategory-enum-type"></a>userExperienceAnalyticsOperatingSystemRestartCategory 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

操作系统重启类别

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知|
|restartWithUpdate|1|使用更新重启|
|restartWithoutUpdate|2|在不更新的情况下重新启动|
|blueScreen|3|蓝屏重启|
|shutdownWithUpdate|4 |通过更新关闭|
|shutdownWithoutUpdate|5 |关机但不更新|
|longPowerButtonPress|6 |长按电源按钮|
|bootError|7 |启动错误|
|update|8 |更新|



