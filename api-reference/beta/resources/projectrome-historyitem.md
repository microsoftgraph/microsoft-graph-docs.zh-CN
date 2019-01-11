---
title: historyItem 资源类型
description: 表示为活动应用程序中的历史记录项。 用户活动表示单个目标应用程序-例如，TV 显示、 文档或视频游戏中当前市场活动中。 当用户启动与该活动时，以指示该活动的开始和结束时间的历史记录项捕获项目。 根据用户重新启动与该活动随着时间的推移，多个历史记录项为单个用户活动记录。
localization_priority: Normal
ms.openlocfilehash: 7eb6d72b55530d1938c9c092dd5b80f54929a3e8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27825772"
---
# <a name="historyitem-resource-type"></a>historyItem 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示为[活动](projectrome-activity.md)应用程序中的历史记录项。 用户活动表示单个目标应用程序-例如，TV 显示、 文档或视频游戏中当前市场活动中。 当用户启动与该活动时，以指示该活动的开始和结束时间的历史记录项捕获项目。 根据用户重新启动与该活动随着时间的推移，多个历史记录项为单个用户活动记录。

当应用程序创建会话时，应是**historyItem**对象添加到**活动**对象以反映用户工作效率期。 每次用户重新启动与活动，新**historyItem**添加到活动以应计用户工作效率。

## <a name="methods"></a>方法

|方法 | 返回类型 | 说明|
|:------|:------------|:-----------|
|[创建或替换 historyItem](../api/projectrome-put-historyitem.md) | [historyItem](projectrome-historyitem.md) | 创建或替换现有**historyItem**为该活动 (upsert)。 ID 需要一个 GUID。|
|[删除 historyItem](../api/projectrome-delete-historyitem.md) | 无内容 | 删除指定的**historyItem**为该活动。|

## <a name="properties"></a>属性

|名称 | 类型 | 说明|
|:----|:-----|:-----------|
|状态 | EnumType | 由服务器设置。 一个用于标识有效对象的状态代码。 值： 活动更新、 删除、 忽略。|
|userTimezone | 字符串 | 可选。 在其中用户的设备用来生成活动位于在活动创建时间的时区。 为了支持跨平台表示形式作为 Olson Id 提供的值。|
|createdDateTime | DateTimeOffset | 由服务器设置。 采用 UTC 的服务器上创建对象时的日期和时间。|
|lastModifiedDateTime | DateTimeOffset | 由服务器设置。 采用 UTC 的服务器上修改对象时的日期和时间。|
|id | 字符串 | 必需。 **HistoryItem**对象的客户端集 GUID。|
|startedDateTime | DateTimeOffset | 必填。 启动**historyItem** （活动会话） 时，日期 UTC 时间。 所需的时间线历史记录。|
|lastActiveDateTime | DateTimeOffset | 可选。 UTC DateTime **historyItem** （活动会话） 的最后一个了解作为活动或完成-如果为空， **historyItem**状态时应日常。|
|expirationDateTime | DateTimeOffset | 可选。 **HistoryItem**会经过硬删除时，日期 UTC 时间。 可以由客户端设置。|
|activeDurationSeconds | int | 可选。 活动用户工作效率的持续时间。 如果未提供，则从**startedDateTime**和**lastActiveDateTime**计算此。|

## <a name="relationships"></a>Relationships

|关系 | 类型 | Description|
|:------------|:-----|:-----------|
|activity| [活动](../resources/projectrome-activity.md) | 可选。 NavigationProperty/包容;导航到关联的活动的属性。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userTimezone",
    "lastActiveDateTime",
    "activeDurationSeconds"
  ],
  "@odata.type": "microsoft.graph.historyItem"
}-->

```json
{
    "status": "String (EnumType)",
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
