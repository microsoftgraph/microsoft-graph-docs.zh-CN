---
title: chatThread 资源类型
description: chatThread 是 Microsoft Teams 中的 chatMessages 集合。
localization_priority: Priority
ms.openlocfilehash: a85b6aea6c48c9295fe88a7412fa7e6b96ee1d3f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521339"
---
# <a name="chatthread-resource-type"></a>chatThread 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

chatThread 是 Microsoft Teams 中的 [chatMessages](chatmessage.md) 集合。

> 目前，可以[在频道内创建](../api/channel-post-chatthreads.md) chatThread。  将来的 API 版本将支持读取现有的 chatThread，以及读取/写入与团队或频道范围外的用户之间的直接聊天。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建线程](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md) |在指定的频道中启动新线程，提供第一条消息。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|rootMessage|[chatMessage](chatmessage.md)| 可为空。|
|chatMessages|[chatMessage](chatmessage.md) 集合| 可为空。|

> 目前这些关系是隐式存在的，但不能读取或写入。  将来的 beta API 版本将支持此功能。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "posts"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatThread"
}-->

```json
{
  "id": "string (identifier)"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatthread.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
