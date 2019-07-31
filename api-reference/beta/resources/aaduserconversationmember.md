---
title: aadUserConversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c4e937d88a1e504c6774b2dcb657dee443d54843
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013631"
---
# <a name="aaduserconversationmember-resource-type"></a>aadUserConversationMember 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[聊天](chat.md)中的 Azure Active Directory 用户。 此类型继承自 [conversationMember](conversationmember.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出聊天成员](../api/conversationmember-list.md) | [conversationmember](conversationmember.md) 集合 | 获取聊天中所有用户的列表。|
|[获取聊天成员](../api/conversationmember-get.md) | [conversationmember](conversationmember.md) | 获取聊天中的单个用户。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|String| 只读。 用户的唯一 ID。|
|displayName| string | 用户的显示名称。 |
|角色| string 集合 | 该用户的角色。 |
|userId| string | 用户的 GUID。 |
|email| string  | 用户的电子邮件地址。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.aadUserConversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string"
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
