---
title: conversationMember 资源类型
description: 代表对话中的用户。
localization_priority: Normal
author: laujan
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 970e64ff358654aafee5b47a229a8425fdc69c9e
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725832"
---
# <a name="conversationmember-resource-type"></a>conversationMember 资源类型

命名空间：microsoft.graph

代表 [团队](team.md)中的用户。
另请参阅 [aadUserConversationMember](aaduserconversationmember.md)。

## <a name="methods"></a>Methods

| 方法       | 返回类型  |说明|
|:---------------|:--------|:----------|
|[列出成员](../api/conversationmember-list.md) | [conversationMember](conversationmember.md) 集合 | 获取包含聊天或频道中所有用户的列表。|
|[获取成员](../api/conversationmember-get.md) | [conversationMember](conversationmember.md) | 获取聊天或频道中的一位用户。|
|[添加成员](../api/conversationmember-add.md) | [conversationMember](conversationmember.md)| 向频道添加成员。|
|[更新成员](../api/conversationmember-update.md) | [conversationMember](conversationmember.md)| 更新频道中的成员。|
|[删除成员](../api/conversationmember-delete.md) | [conversationMember](conversationmember.md)| 删除频道中的成员。|

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

