---
title: chatMessageReaction 资源类型
description: '表示对 chatMessage 实体的一种反应。 '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: bc7a3a5cbff2aee1191383ac18128e97075b4b99
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721619"
---
# <a name="chatmessagereaction-resource-type"></a>chatMessageReaction 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示对 [chatMessage 实体](chatmessage.md) 的一种反应。 

类型实体作为 `chatMessageReaction` [chatMessage](chatmessage.md)实体的一部分作为[获取](../api/channel-get-message.md)频道消息 API 的一部分返回。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。 例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`|
|reactionType|String|支持的值是 `like` ， ， ， ， `angry` `sad` `laugh` `heart` `surprised` 。 |
|user|[identitySet](identityset.md)|对邮件做出响应的用户。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatMessageReaction",
  "baseType": null
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "reactionType": "String",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chatMessageReaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


