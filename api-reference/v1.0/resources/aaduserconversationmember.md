---
title: aadUserConversationMember 资源类型
description: 表示聊天或频道中的 Azure Active Directory 用户。
ms.localizationpriority: high
author: akjo
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9aa64f0f6cfc6ea3571b0c2a1995c57644db4074
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59007325"
---
# <a name="aaduserconversationmember-resource-type"></a>aadUserConversationMember 资源类型

命名空间：microsoft.graph

表示[团队](team.md)、[频道](channel.md)或[聊天](chat.md)中的 Azure Active Directory 用户。
此类型继承自 [conversationMember](conversationmember.md)。

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
|[列出聊天成员](../api/chat-list-members.md) | [conversationMember](conversationmember.md) 集合 | 获取聊天中的所有成员列表。|
|[添加聊天成员](../api/chat-post-members.md) | 位置标头 | 向聊天添加成员。| 
|[获取聊天成员](../api/chat-get-members.md) | [conversationMember](conversationmember.md) | 获取聊天中的成员。|
|[删除聊天成员](../api/chat-delete-members.md) | 无 | 从聊天中删除成员。| 

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
|:---------------|:--------|:----------|
|id|String| 只读。用户的唯一 ID。|
|displayName| string | 用户的显示名称。 |
|角色| string 集合 | 该用户的角色。 |
|userId| string | 用户的 GUID。 |
|email| string  | 用户的电子邮件地址。 |
|tenantId| string  | Azure AD 用户从属的 TenantId。 |
|visibleHistoryStartDateTime| DateTimeOffset  | 表示对话历史久远程度的时间戳与对话成员共享。 此属性只对聊天成员可设置。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.aadUserConversationMember",
  "baseType": "microsoft.graph.conversationMember",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aadUserConversationMember",
  "id": "string (identifier)",
  "displayName" : "string",
  "visibleHistoryStartDateTime": "string (timestamp)",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string",
  "tenantId": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "aadUserConversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

