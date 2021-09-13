---
title: chatMessageMention 资源类型
description: '表示 chatMessage 实体中的提及。 提及内容可以提及用户、团队、机器人或频道。 '
ms.localizationpriority: medium
author: RamjotSingh
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8b458393d73c7547dda1638e86c2fa4782e3b4d4
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109421"
---
# <a name="chatmessagemention-resource-type"></a>chatMessageMention 资源类型

命名空间：microsoft.graph

表示 [chatMessage 实体中的](chatmessage.md) 提及。 提及的内容可以是用户[、](user.md)[团队、](team.md)机器人或[频道](channel.md)。 

在包含 **一个或多个提及内容的 chatMessage** 对象中，消息正文 **内容** 属性表示 HTML 格式的聊天消息。 它将每个 **提及的内容的 mentionText** 包含在 HTML 元素中，并包含对应于提及项 `at` 的 `id` **id** 属性的属性。

例如，聊天消息包含两个提及内容，分别包含提及文本"Megan"和"Alex"。 其 body **content** 属性 `at` 指定两个提及项的元素，如下所示：

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

在 **content** 属性中，第一个提及具有 HTML `id` 属性 0。 这对应于 **chatMessageMention** 的第一个实例的 **id** 属性，这也是 0。

第二个提及具有与第二个实例的 id 属性匹配的属性 `id` 1，即 1。 

有关示例的更完整上下文，请参阅 [列表频道消息回复](../api/chatmessage-list-replies.md#example)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|Int32|指定的 **chatMessage** 中提及的实体的索引。 匹配邮件正文中相应标记中的 `<at id="{index}">` {index} 值。|
|mentionText|string|用于表示提及的字符串。 例如，用户的显示名称，一个团队名称。|
|提及|[chatMessageIdentitySet](chatmessagementionedidentityset.md)|包含 (用户、应用程序、团队或频道) 实体@mentioned。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": 1024,
  "mentionText": "string",
  "mentioned": {"@odata.type": "microsoft.graph.chatMessageMentionedIdentitySet"}
 }
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


