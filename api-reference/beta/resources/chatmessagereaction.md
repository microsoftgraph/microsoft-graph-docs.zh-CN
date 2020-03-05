---
title: chatMessageReaction 资源类型
description: '表示对了 chatmessage 实体的反应。 '
localization_priority: Normal
doc_type: resourcePageType
author: RamjotSingh
ms.prod: microsoft-teams
ms.openlocfilehash: cb26a46a3669b721184399036fa80e4a6b291ec8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507689"
---
# <a name="chatmessagereaction-resource-type"></a>chatMessageReaction 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示对[了 chatmessage](chatmessage.md)实体的反应。 

作为[了 chatmessage](chatmessage.md)实体的`chatMessageReaction`一部分，类型的实体作为[Get 信道消息](../api/channel-get-message.md)API 的一部分返回。

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|createdDateTime|DateTimeOffset|时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`|
|reactionType|String|受支持的`like`值`angry`为`sad`、 `laugh`、 `heart`、 `surprised`、、。 |
|user|[identitySet](identityset.md)|Reacted 邮件的用户。|

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
