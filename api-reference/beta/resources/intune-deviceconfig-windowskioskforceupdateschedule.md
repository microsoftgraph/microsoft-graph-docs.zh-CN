---
title: windowsKioskForceUpdateSchedule 资源类型
description: 展台设备的 Windows 10 强制更新计划。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4e308d0ea6fc8015281515ce0d60d859ed326c16
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370886"
---
# <a name="windowskioskforceupdateschedule-resource-type"></a>windowsKioskForceUpdateSchedule 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

展台设备的 Windows 10 强制更新计划。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startDateTime|DateTimeOffset|强制重启的开始时间。|
|recurrence|[windows10AppsUpdateRecurrence](../resources/intune-deviceconfig-windows10appsupdaterecurrence.md)|定期计划。 可取值为：`none`、`daily`、`weekly`、`monthly`。|
|dayofWeek|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|一周中的某一天。 可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。|
|dayofMonth|Int32|月中的某一天。 有效值为1至31|
|runImmediatelyIfAfterStartDateTime|Boolean|如果为 true, 则在 StartDateTime 为过去时立即运行任务, 否则在下一个定期运行。|

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



