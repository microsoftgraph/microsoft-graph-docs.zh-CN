---
title: conversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Normal
author: clearab
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2a8e4c94681065d9686e9f17888d3abf35885a65
ms.sourcegitcommit: f9f95402b8a15152ede90dd736b03d532204fc2e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/11/2020
ms.locfileid: "49658040"
---
# <a name="conversationmember-resource-type"></a>conversationMember 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[聊天](chat.md)或[频道](channel.md)中的用户。
另请参阅 [aadUserConversationMember](aaduserconversationmember.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出聊天成员](../api/conversationmember-list.md) | [conversationMember](conversationmember.md) 集合 | 获取聊天中所有用户的列表。|
|[获取聊天成员](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | 获取聊天中的单个用户。|
|[列出团队成员](../api/team-list-members.md)|[conversationMember](../resources/conversationmember.md) 集合|获取此团队中的成员列表。|
|[获取团队成员](../api/team-get-members.md) | [conversationMember](conversationmember.md) 集合 | 获取团队中的成员。|
|[添加团队成员](../api/team-post-members.md)|[conversationMember](../resources/conversationmember.md)|向团队中添加新成员。|
|[批量添加团队成员](../api/conversationmembers-add.md)|[actionResultPart](../resources/actionresultpart.md) 集合|在单个请求中向团队添加多个成员。|
|[更新团队成员的角色](../api/team-update-members.md)|[conversationMember](../resources/conversationmember.md)|将成员更改为所有者或返回为常规成员。|
|[删除团队成员](../api/team-delete-members.md)|无|删除团队中的一个现有成员。|
|[获取频道成员](../api/channel-get-members.md) | [conversationMember](conversationmember.md) 集合 | 获取频道中的成员。|
|[创建频道成员](../api/channel-post-members.md) | [conversationMember](conversationmember.md) | 向频道添加成员。 仅支持 membershipType 为 `private` 的 `channel`。|
|[更新频道成员角色](../api/channel-update-members.md) | [conversationMember](conversationmember.md) | 更新频道成员的属性。 仅支持 membershipType 为 `private` 的频道。|
|[删除频道成员](../api/channel-delete-members.md) | 无 | 从频道中删除一个成员。 仅支持用于 `private` 的 `channelType`。|



## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 用户的唯一 ID。|
|displayName| string | 用户的显示名称。 |
|角色| string 集合 | 该用户的角色。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "roles": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


