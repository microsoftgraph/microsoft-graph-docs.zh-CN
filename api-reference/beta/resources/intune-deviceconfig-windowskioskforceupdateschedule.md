---
title: windowsKioskForceUpdateSchedule 资源类型
description: Windows 10展台设备强制更新计划。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 18b6938740db45281ef06529b8b98546fa1f2d169313a3c263a7d616140ea081
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54226333"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a>windowsKioskForceUpdateSchedule 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 10展台设备强制更新计划。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startDateTime|DateTimeOffset|强制重启的开始时间。|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|定期计划。 可取值为：`none`、`daily`、`weekly`、`monthly`。|
|dayofWeek|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|星期数。 可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。|
|dayofMonth|Int32|月中的一天。 有效值为 1 到 31|
|runImmediatelyIfAfterStartDateTime|布尔值|如果为 true，则如果 StartDateTime 过去，则立即运行该任务，否则，下次重复执行。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskForceUpdateSchedule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskForceUpdateSchedule",
  "startDateTime": "String (timestamp)",
  "recurrence": "String",
  "dayofWeek": "String",
  "dayofMonth": 1024,
  "runImmediatelyIfAfterStartDateTime": true
}
```




