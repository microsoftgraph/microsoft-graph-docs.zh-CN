---
title: conversationMember 资源类型
description: 表示对话中的用户。
ms.localizationpriority: medium
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: fa41b65aa3cfdd894795337430622aebbf80c45a
ms.sourcegitcommit: 2132198551c7d1f37474debab471f612a3e35a08
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/17/2022
ms.locfileid: "66141234"
---
# <a name="conversationmember-resource-type"></a>conversationMember 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 [团队](team.md) 、 [频道](channel.md) 或 [聊天](chat.md)中的用户。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出团队成员](../api/team-list-members.md)|[conversationMember](../resources/conversationmember.md) 集合|获取此团队中的成员列表。|
|[添加团队成员](../api/team-post-members.md)|[conversationMember](../resources/conversationmember.md)|向团队中添加新成员。|
|[批量添加团队成员。](../api/conversationmembers-add.md)|[actionResultPart](../resources/actionresultpart.md) 集合|在单个请求中将多个成员添加到团队中。|
|[获取团队成员](../api/team-get-members.md) | [conversationMember](conversationmember.md) 集合 | 获取团队中的成员。|
|[更新成员角色](../api/team-update-members.md)|[conversationMember](../resources/conversationmember.md)|将成员更改为所有者或返回为常规成员。|
|[删除团队成员](../api/team-delete-members.md)|无|删除团队中的一个现有成员。|
|[列出频道成员](../api/channel-list-members.md) | [conversationMember](conversationmember.md) 集合 | 获取频道中的所有成员列表。|
|[添加频道成员](../api/channel-post-members.md) | [conversationMember](conversationmember.md) | 向频道添加成员。 仅支持 membershipType 为 `private` 的 `channel`。|
|[获取频道成员](../api/channel-get-members.md) | [conversationMember](conversationmember.md) 集合 | 获取频道中的成员。|
|[更新频道成员角色](../api/channel-update-members.md) | [conversationMember](conversationmember.md) | 更新频道成员的属性。 仅支持 membershipType 为 `private` 的频道。|
|[删除频道成员](../api/channel-delete-members.md) | 无 | 从频道中删除一个成员。 仅支持用于 `private` 的 `channelType`。|
|[列出聊天成员](../api/chat-list-members.md) | [conversationMember](conversationmember.md) 集合 | 获取聊天中的所有成员列表。|
|[添加聊天成员](../api/chat-post-members.md) | 位置标头 | 向聊天添加成员。| 
|[获取聊天成员](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | 获取聊天中的成员。|
|[删除聊天成员](../api/chat-delete-members.md) | 无 | 从聊天中删除成员。| 

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|String| 只读。用户的唯一 ID。|
|displayName| string | 用户的显示名称。 |
|角色| string 集合 | 该用户的角色。 此属性仅在相关时包含其他限定符 -例如，如果成员具有 `owner` 权限， **则角色** 属性包含 `owner` 为值之一。 同样，如果成员是来宾， **则角色** 属性包含 `guest` 为值之一。 基本成员不应在 **角色** 属性中指定任何值。 |
|visibleHistoryStartDateTime| DateTimeOffset | 表示对话历史久远程度的时间戳与对话成员共享。 此属性只对聊天成员可设置。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.conversationMember",
  "id": "String (identifier)",
  "roles": [
    "String"
  ],
  "displayName": "String",
  "visibleHistoryStartDateTime": "String (timestamp)"
}
```

## <a name="see-also"></a>另请参阅

- [aadUserConversationMember](aaduserconversationmember.md)
- [skypeForBusinessUserConversationMember](skypeForBusinessUserConversationMember.md)
- [anonymousGuestConversationMember](anonymousGuestConversationMember.md)
- [skypeUserConversationMember](skypeUserConversationMember.md)
- [microsoftAccountUserConversationMember](microsoftAccountUserConversationMember.md)

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


