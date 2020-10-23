---
title: aadUserConversationMember 资源类型
description: 表示聊天或频道中的 Azure Active Directory 用户。
localization_priority: Priority
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 6057c8cf71ce0f8d71632267d3790c39b69b1eb1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48735762"
---
# <a name="aaduserconversationmember-resource-type"></a>aadUserConversationMember 资源类型

命名空间：microsoft.graph

表示[团队](team.md)中的 Azure Active Directory 用户。
此类型继承自 [conversationMember](conversationmember.md)。

## <a name="methods"></a>方法

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[List members](../api/conversationmember-list.md) | [conversationMember](conversationmember.md) 集合 | 获取包含聊天或频道中所有用户的列表。|
|[获取成员](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | 获取聊天或频道中的单个用户。|
|[添加成员](../api/conversationmember-add.md) | [conversationMember](conversationmember.md)| 向频道添加成员。|
|[更新成员](../api/conversationmember-update.md) | [conversationMember](conversationmember.md)| 更新频道中的成员。|
|[删除成员](../api/conversationmember-delete.md) | [conversationMember](conversationmember.md)| 删除频道中的成员。|

## <a name="properties"></a>属性

| 属性   | 类型 |说明|
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

