---
title: chatMessageReaction 资源类型
description: '代表 chatMessage 实体的反应。 '
ms.openlocfilehash: 1ad1f7948405a8891ec9aa13065b71108e9c47c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049183"
---
# <a name="chatmessagereaction-resource-type"></a>chatMessageReaction 资源类型

代表[chatMessage](chatmessage.md)实体的反应。 

实体类型的`chatMessageReaction`返回作为一部分[获取通道消息](../api/channel-get-message.md)API，作为[chatMessage](chatmessage.md)实体的一部分。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|reactionType|string| 反应的类型。 计划的值包括： <br><ul><li>像-像一条消息，内容为空在这种情况下。</li><li>Emoji-Emoji 反应。 内容设置为 unicode 值的 emoji。</li><li>标签-内容设置为中标签的字符串。</li></ul>|
|createdDateTime|dateTimeOffset|ISO-8601 格式中的根消息的 UTC 时间戳。|
|user|identitySet|反应到邮件用户。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "content"
  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageReaction"
}-->

```json
{
  "reactionType": "string ",
  "createdDateTime": "string (timestamp)",
  "user": {"@odata.type": "microsoft.graph.identitySet"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message reaction resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
