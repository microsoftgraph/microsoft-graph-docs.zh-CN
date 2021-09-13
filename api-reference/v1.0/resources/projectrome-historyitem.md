---
title: historyItem 资源类型
description: 表示应用中活动的历史记录项。 用户活动表示应用中的单个目标，例如，电视、文档或游戏中的当前活动。 当用户参与该活动时，该活动将捕获为指示该活动的开始时间和结束时间的历史项。 随着用户随着时间的过去重新参与该活动，将针对单个用户活动记录多个历史记录项。
ms.localizationpriority: medium
ms.prod: project-rome
author: ailae
doc_type: resourcePageType
ms.openlocfilehash: 63c99a470c71b572763de4d38cf2c16f4a202a7b
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59028784"
---
# <a name="historyitem-resource-type"></a>historyItem 资源类型

命名空间：microsoft.graph

表示应用中活动的 [历史记录](projectrome-activity.md) 项。 用户活动表示应用中的单个目标，例如，电视、文档或游戏中的当前活动。 当用户参与该活动时，该活动将捕获为指示该活动的开始时间和结束时间的历史项。 随着用户随着时间的过去重新参与该活动，将针对单个用户活动记录多个历史记录项。

当应用创建会话时，应向活动对象添加 **historyItem** 对象以反映用户参与的时间段。 每次用户重新参与活动时，会向活动添加一个新的 **historyItem，** 以增加用户参与度。

## <a name="methods"></a>方法

|方法 | 返回类型 | 说明|
|:------|:------------|:-----------|
|[创建或替换 historyItem](../api/projectrome-put-historyitem.md) | [historyItem](projectrome-historyitem.md) | 创建或替换活动的现有 **historyItem** (upsert) 。 ID 需要为 GUID。|
|[删除 historyItem](../api/projectrome-delete-historyitem.md) | 无内容 | 删除该活动的指定 **historyItem。**|

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|状态 | status | 由服务器设置。 用于标识有效对象的状态代码。 值：活动、已更新、已删除、已忽略。|
|userTimezone | String | 可选。 用户用于生成活动的设备在活动创建时所在的时区。 作为 Olson ID 提供以支持跨平台表示的值。|
|createdDateTime | DateTimeOffset | 由服务器设置。 在服务器上创建对象时的日期/时间（UTC 时间）。|
|lastModifiedDateTime | DateTimeOffset | 由服务器设置。 在服务器上修改对象的 DateTime（UTC 时间）。|
|id | String | 必填。 **historyItem** 对象的客户端集 GUID。|
|startedDateTime | DateTimeOffset | 必需。 UTC **DateTime，当启动 historyItem** (活动会话) 的时间。 时间线历史记录的必需项。|
|lastActiveDateTime | DateTimeOffset | 可选。 UTC DateTime **上次将 historyItem** (活动会话) 活动或已完成的时间 - 如果为 null， **则 historyItem** 状态应为"正在进行"。|
|expirationDateTime | DateTimeOffset | 可选。 UTC DateTime **historyItem** 将进行硬删除的时间。 客户端可以设置。|
|activeDurationSeconds | int | 可选。 活动用户参与的持续时间。 如果未提供，则从 **startedDateTime** 和 **lastActiveDateTime 计算得来**。|

## <a name="relationships"></a>关系

|关系 | 类型 | 说明|
|:------------|:-----|:-----------|
|活动| [userActivity](../resources/projectrome-activity.md) | 可选。 NavigationProperty/包含;导航属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.activityHistoryItem",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
    "status": "active | updated | deleted | ignored",
    "createdDateTime": "DateTimeOffset",
    "lastModifiedDateTime": "DateTimeOffset",
    "id": "String",
    "expirationDateTime": "DateTimeOffset",
    "startedDateTime": "DateTimeOffset",
    "userTimezone": "String",
    "lastActiveDateTime": "DateTimeOffset",
    "activeDurationSeconds":"int"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "historyitem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

