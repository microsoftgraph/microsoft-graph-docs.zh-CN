---
title: 聊天资源类型
description: 聊天是一个或多个参与者之间的 Chatmessages 集合的集合。
author: clearab
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 61c23e32d455dd18af639dad31806d54d9e8bd07
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974022"
---
# <a name="chat-resource-type"></a>聊天资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

聊天是一个或多个参与者之间的[chatmessages 集合](chatmessage.md)的集合。 参与者可以是用户或应用程序。

## <a name="methods"></a>方法

|  方法       |  返回类型  | 说明|
|:---------------|:--------|:----------|
|[列出聊天](../api/chat-list.md) | [聊天](channel.md)收藏 | 获取用户所属的聊天列表。|
|[获取聊天](../api/chat-get.md) | [参与](channel.md) | 读取聊天的属性和关系。|
|[列出聊天成员](../api/conversationmember-list.md) | [conversationmember](conversationmember.md)集合 | 获取聊天中所有用户的列表。|
|[获取聊天成员](../api/conversationmember-get.md) | [conversationmember](conversationmember.md) | 获取聊天中的单个用户。|
|[列出聊天中的消息](../api/chatmessage-list.md)  | [chatMessage](../resources/chatmessage.md) | 获取一对一聊天或群组聊天中的消息。 |
|[获取聊天中的消息](../api/chatmessage-get.md)  | [chatMessage](../resources/chatmessage.md) | 获取聊天中的单个消息。 |

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
| id| String| 聊天的唯一标识符。 只读。|
| topic| String|  Optional聊天的主题或主题。 仅适用于组聊天。|
| createdDateTime| dateTimeOffset|  聊天的创建日期和时间。 只读。|
| lastUpdatedDateTime| dateTimeOffset|  更新聊天的日期和时间。 只读。|

## <a name="relationships"></a>关系

| 关系 | 类型 |说明|
|:---------------|:--------|:----------|
| installedApps | [teamsAppInstallation](teamsappinstallation.md) 集合 | 聊天中所有应用的集合。 可为 Null。 |
| members | [conversationMember](conversationmember.md)集合 | 聊天中所有人员的集合。 可为 Null。 |
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
  "topic": "string",
  "createdDateTime": "dateTimeOffset",
  "lastUpdatedDateTime": "dateTimeOffset"
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
