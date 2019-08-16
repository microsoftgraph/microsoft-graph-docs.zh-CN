---
title: conversationMember 资源类型
description: 表示对话中的用户。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ca5115922dfb40239b8ca290a39f3c5953d4e4ed
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973973"
---
# <a name="conversationmember-resource-type"></a>conversationMember 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示[聊天](chat.md)中的用户。

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

## <a name="relationships"></a>关系

无

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