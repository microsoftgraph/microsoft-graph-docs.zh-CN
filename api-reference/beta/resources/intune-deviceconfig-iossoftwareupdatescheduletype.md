---
title: iosSoftwareUpdateScheduleType 枚举类型
description: 更新 iOS 软件更新的计划类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 58a59e32fd75a99c9585d9c22115620b8a4aad20
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526302"
---
# <a name="iossoftwareupdatescheduletype-enum-type"></a>iosSoftwareUpdateScheduleType 枚举类型

命名空间： microsoft. graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

更新 iOS 软件更新的计划类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|updateOutsideOfActiveHours|0|更新为主动时段之外的。|
|alwaysUpdate|1 |时刻更新。|
|updateDuringTimeWindows|2 |在时间时段内更新。|
|updateOutsideOfTimeWindows|3 |在时段外更新。|



