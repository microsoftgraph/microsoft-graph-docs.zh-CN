---
title: chatMessageReaction 资源类型
description: '表示对了 chatmessage 实体的反应。 '
localization_priority: Normal
ms.openlocfilehash: 5020653ef02c1604aece46f3ff2c7ea1c82a75ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460637"
---
# <a name="chatmessagereaction-resource-type"></a>chatMessageReaction 资源类型

表示对[了 chatmessage](chatmessage.md)实体的反应。 

类型`chatMessageReaction`的实体作为[Get 信道消息](../api/channel-get-message.md)API 的一部分返回, 作为[了 chatmessage](chatmessage.md)实体的一部分。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|reactionType|字符串| 反应的类型。 计划的值包括: <br><ul><li>类似于邮件, 在这种情况下内容为空。</li><li>表情符号-表情符号反应。 将内容设置为表情符号的 unicode 值。</li><li>标签-内容设置为标签中的字符串。</li></ul>|
|createdDateTime|dateTimeOffset|以 ISO-8601 格式表示的根邮件的 UTC 时间戳。|
|user|identitySet|reacted 邮件的用户。|

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
