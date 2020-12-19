---
title: conversationMember 资源类型
description: 代表对话中的用户。
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 2d2e44349f7896dfed0d0dff455e9afd0ac65772
ms.sourcegitcommit: 0d4377b0153bc339ab7b3b1a6ee4d52848b622d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49714275"
---
# <a name="conversationmember-resource-type"></a>conversationMember 资源类型

命名空间：microsoft.graph

表示[团队、频道](team.md)[或聊天](channel.md)中的[用户](chat.md)。
另请参阅 [aadUserConversationMember](aaduserconversationmember.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出团队成员](../api/team-list-members.md)|[conversationMember](../resources/conversationmember.md) 集合|获取此团队中的成员列表。|
|[添加团队成员](../api/team-post-members.md)|[conversationMember](../resources/conversationmember.md)|向团队中添加新成员。|
|[获取团队成员](../api/team-get-members.md) | [conversationMember](conversationmember.md) 集合 | 获取团队中的成员。|
|[更新成员角色](../api/team-update-members.md)|[conversationMember](../resources/conversationmember.md)|将成员更改为所有者或返回为常规成员。|
|[删除团队成员](../api/team-delete-members.md)|无|删除团队中的一个现有成员。|
|[列出频道成员](../api/channel-list-members.md) | [conversationMember](conversationmember.md) 集合 | 获取频道中的所有成员列表。|
|[添加频道成员](../api/channel-post-members.md) | [conversationMember](conversationmember.md) | 向频道添加成员。 仅支持 membershipType 为 `private` 的 `channel`。|
|[获取频道成员](../api/channel-get-members.md) | [conversationMember](conversationmember.md) 集合 | 获取频道中的成员。|
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

