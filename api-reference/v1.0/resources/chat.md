---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 Chatmessages 集合的集合。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7f9cc43442e077dfe245fa8422b954859bf1c569
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564068"
---
# <a name="chat-resource-type"></a>聊天资源类型

命名空间：microsoft.graph

聊天是一个或多个参与者之间的 [chatmessages 集合](chatmessage.md) 的集合。 参与者可以是用户或应用程序。

## <a name="methods"></a>方法

|  方法       |  返回类型  | 说明|
|:---------------|:--------|:----------|
|[在用户和应用之间获取聊天](../api/userscopeteamsappinstallation-get-chat.md) | [聊天](chat.md)| 在用户和应用之间获取一对一聊天 | 

>**注意：** 使用应用程序权限时，请务必了解如何获取聊天 ID。 由于不支持列出具有应用程序权限的聊天，因此并非所有方案都可行。 可以获取具有委派权限的聊天 Id，也可以通过应用程序权限获取 [/chats/getAllMessages 的更改通知](../api/subscription-post-subscriptions.md) 。

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
| id| String| 聊天的唯一标识符。 只读。|


## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
| messages | [chatMessage](chatmessage.md) 集合 | 聊天中所有邮件的集合。 可为 Null。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chat"
}-->

```json
{
  "id": "string (identifier)",
}
```

## <a name="see-also"></a>另请参阅

- [频道](channel.md)
- [chatMessage](chatmessage.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->


