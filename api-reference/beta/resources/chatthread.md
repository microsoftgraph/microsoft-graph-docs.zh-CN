---
title: chatThread 资源类型
description: chatThread 是 Microsoft Teams 中的 chatMessages 集合。
localization_priority: Priority
ms.openlocfilehash: 19365109c2008d52d3597b3d23fc1baefa5cfd1c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399603"
---
# <a name="chatthread-resource-type"></a>chatThread 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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
<!-- {
  "type": "#page.annotation",
  "description": "chatThread resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
