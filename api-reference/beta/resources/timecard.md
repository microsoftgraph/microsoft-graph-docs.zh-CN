---
title: timecard 资源类型
description: 计划中的考勤卡条目。
author: akumar39
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType_
ms.openlocfilehash: 25818e091ac2d4f6590fd7ea2c395752d0238bd0
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786383"
---
# <a name="timecard-resource-type"></a>timecard 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示计划中的一个考勤卡条目。

## <a name="methods"></a>方法

| 方法       | 返回类型  |Description|
|:---------------|:--------|:----------|
|[List](../api/timecard-list.md) | [timeCard](timecard.md) 集合 | 获取此 **计划中的 timecard** 对象列表。|
|[创建](../api/timecard-post.md) | [timeCard](timecard.md) | 创建新的 **时间卡** 对象。|
|[获取](../api/timecard-get.md) | [timeCard](timecard.md) | 按 ID **获取** 时间卡对象。|
|[Replace](../api/timecard-replace.md) | 无 | 替换 **一个时间卡** 对象。|
|[删除](../api/timecard-delete.md) | 无 | 从 **计划中删除** 一个时间卡对象。|
|[clockIn](../api/timecard-clockin.md) | [timeCard](timecard.md) | Clock in to start a **timecard**.|
|[clockOut](../api/timecard-clockout.md) | 无 | 时钟以结束打开的 **Timecard**。|
|[startBreak](../api/timecard-startbreak.md) | 无 | 启动特定时间卡 中的 **timeCardBreak** **。**|
|[endBreak](../api/timecard-endbreak.md) | 无 | 结束特定时间卡中打开的 **timeCardBreak。** |
|[confirmTimeCard](../api/timecard-confirm.md) | 无 | 确认 **一条时间卡** 记录。|

## <a name="properties"></a>属性
|属性               |类型           |说明                                                                |
|-----------------------|---------------|---------------------------------------------------------------------------|
| id                    |`string`  |timeCard的 ID。|
| userId                    |`string` |**timeCard** 所属的用户 ID。 |
| state                 |`timeCardState`  | **timeCard** 在其生命周期中的当前状态。可能的值是 `clockedIn` `onBreak` `clockedOut` ：、、、。 `unknownFutureValue`|
| clockInEvent       |[timeCardEvent](../resources/timecardevent.md)    | timeCard 的 **时钟事件**。 |
| clockOutEvent                 |[timeCardEvent](../resources/timecardevent.md)  |timeCard 的 **时钟出事件**。 |
| notes                 | [itemBody](itembody.md)  |有关 **timeCard 的注释**。 |
| breaks    |[timeCardBreak](timecardbreak.md) 集合  |与 **timeCard** 关联的中断列表。|
| originalEntry| [timeCardEntry](../resources/timecardentry.md) | 用户编辑之前 timeCard 的原始 **timeCardEntry。**  |
| confirmedBy |`confirmedBy`    | 指示此 **timeCard** 条目是否得到确认。 可取值为：`none`、`user`、`manager`、`unknownFutureValue`。|
|createdDateTime|`Edm.dateTimeOffset`| 创建 **timeCard** 的时间戳。 |
|createdBy|`IdentitySet`| 创建实体的人的标识。 |
|lastModifiedDateTime|`dateTimeOffset`| 上次修改 **timeCard** 的时间戳。|
|lastModifiedBy| `IdentitySet`| 上次修改实体的人的标识。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.timeCard",
   "baseType":"microsoft.graph.changeTrackedEntity"
}-->

```json
{
  "userId": "string (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "lastModifiedBy": {"@odata.type":"microsoft.graph.identitySet"},
  "clockInEvent" : {"@odata.type":"microsoft.graph.timeCardEvent"},
  "clockOutEvent" : {"@odata.type":"microsoft.graph.timeCardEvent"},
  "notes" : {"@odata.type":"microsoft.graph.itemBody"},
  "breaks" : [{"@odata.type":"microsoft.graph.timeCardEvent"}],
  "originalEntry" : {"@odata.type":"microsoft.graph.timeCardEntry"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "timeCard resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
