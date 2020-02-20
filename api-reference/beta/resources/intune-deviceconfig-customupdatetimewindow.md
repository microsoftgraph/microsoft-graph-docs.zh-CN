---
title: customUpdateTimeWindow 资源类型
description: 自定义更新时间窗口
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d412f568a48c4da7b41d56b44180ac5200961238
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42160935"
---
# <a name="customupdatetimewindow-resource-type"></a>customUpdateTimeWindow 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

自定义更新时间窗口

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|startDay|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|时间范围的开始日期。 可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。|
|endDay|[dayOfWeek](../resources/intune-deviceconfig-dayofweek.md)|时间范围的结束日期。 可取值为：`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday` 或 `saturday`。|
|startTime|TimeOfDay|时间范围的开始时间|
|endTime|TimeOfDay|时间范围的结束时间|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customUpdateTimeWindow"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customUpdateTimeWindow",
  "startDay": "String",
  "endDay": "String",
  "startTime": "String (time of day)",
  "endTime": "String (time of day)"
}
```



