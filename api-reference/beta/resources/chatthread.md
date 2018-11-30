---
title: chatThread 资源类型
description: ChatThread 是 chatMessages 中的 Microsoft 团队的集合。
ms.openlocfilehash: ef8f118ae4354a5e4197802708aecfa1fb6f8cb8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048298"
---
# <a name="chatthread-resource-type"></a>chatThread 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

ChatThread 是[chatMessages](chatmessage.md)中的 Microsoft 团队的集合。

> 目前，chatThreads 可以是[在通道中创建](../api/channel-post-chatthreads.md)。  未来 API 版本将支持读取现有 chatThreads，以及读取/写入直接聊天之间的团队或通道范围之外的用户。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[创建线程](../api/channel-post-chatthreads.md) | [chatThread](chatthread.md) |在指定的通道，提供第一条消息中启动一个新的线程。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。|

## <a name="relationships"></a>Relationships
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|rootMessage|[chatMessage](chatmessage.md)| 可为 Null。|
|chatMessages|[chatMessage](chatmessage.md)集合| 可为 Null。|

> 当前这些关系存在隐式，但不能读取或写入。  将来 beta API 版本将支持此功能。

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
  "id": "string (identifier)",
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
