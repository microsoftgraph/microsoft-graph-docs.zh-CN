---
title: historyItem 资源类型
description: 表示应用中的活动的历史记录项。 用户活动表示应用程序中的单个目标, 例如电视节目、文档或视频游戏中的当前市场活动。 当用户参与该活动时, 会将该预订作为历史项目进行捕获, 以指示该活动的开始时间和结束时间。 随着时间的推移, 用户随着时间的推移而重新参与该活动, 会为单个用户活动记录多个历史记录项目。
localization_priority: Normal
ms.prod: project-rome
author: ''
doc_type: resourcePageType
ms.openlocfilehash: 38cba88a5605e1c67ae84b684425db3c71f5d51c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035005"
---
# <a name="historyitem-resource-type"></a>historyItem 资源类型

表示应用中的[活动](projectrome-activity.md)的历史记录项。 用户活动表示应用程序中的单个目标, 例如电视节目、文档或视频游戏中的当前市场活动。 当用户参与该活动时, 会将该预订作为历史项目进行捕获, 以指示该活动的开始时间和结束时间。 随着时间的推移, 用户随着时间的推移而重新参与该活动, 会为单个用户活动记录多个历史记录项目。

当应用程序创建会话时, 应将一个**historyItem**对象添加到**活动**对象, 以反映用户参与的时段。 用户每次重新参与活动时, 都会向活动中添加一个新的**historyItem**以计入用户约定。

## <a name="methods"></a>方法

|方法 | 返回类型 | 说明|
|:------|:------------|:-----------|
|[创建或替换 historyItem](../api/projectrome-put-historyitem.md) | [historyItem](projectrome-historyitem.md) | 创建或替换该活动的现有**historyItem** (upsert)。 ID 必须是 GUID。|
|[删除 historyItem](../api/projectrome-delete-historyitem.md) | 无内容 | 删除该活动的指定**historyItem** 。|

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|状态 | status | 由服务器进行设置。 用于标识有效对象的状态代码。 值: 活动、已更新、已删除、已忽略。|
|userTimezone | String | 可选。 用于生成活动的用户设备所在的时区位于活动创建时间。 作为 Olson Id 提供的值, 以便支持跨平台表示形式。|
|createdDateTime | DateTimeOffset | 由服务器进行设置。 在服务器上创建对象时的 UTC 时间 (UTC)。|
|lastModifiedDateTime | DateTimeOffset | 由服务器进行设置。 在服务器上修改对象时的 UTC 时间 (UTC)。|
|id | String | 必需。 客户端集的**historyItem**对象的 GUID。|
|startedDateTime | DateTimeOffset | 必需。 **HistoryItem** (活动会话) 启动时的 UTC 日期时间。 对于时间线历史记录是必需的。|
|lastActiveDateTime | DateTimeOffset | 可选。 UTC DateTime 如果**historyItem** (活动会话) 上次被视为活动或已完成-如果为 null, 则**historyItem**状态应为 "正在进行"。|
|expirationDateTime | DateTimeOffset | 可选。 **HistoryItem**将被硬删除时的 UTC 日期时间。 可由客户端进行设置。|
|activeDurationSeconds | int | 可选。 活动用户约定的持续时间。 如果未提供, 则从**startedDateTime**和**lastActiveDateTime**计算。|

## <a name="relationships"></a>关系

|关系 | 类型 | 说明|
|:------------|:-----|:-----------|
|activity| [Useractivity.readwrite.createdbyapp](../resources/projectrome-activity.md) | 可选。 NavigationProperty/包含;指向关联活动的导航属性。|

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
