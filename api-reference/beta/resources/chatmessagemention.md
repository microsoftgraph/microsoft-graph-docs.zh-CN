---
title: chatMessageMention 资源类型
description: '表示 chatMessage 实体中的提及。 这些提及适用于用户、团队、机器人或频道。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: e4b6ce12589525e7ddb471f5744d68539c905f3d
ms.sourcegitcommit: 239db9e961e42b505f52de9859963a9136935f2f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/20/2020
ms.locfileid: "46819719"
---
# <a name="chatmessagemention-resource-type"></a>chatMessageMention 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示 chatMessage 实体中的 [提及](chatmessage.md) 。 提及可以是对用户[、](user.md)[团队、机](team.md)器人[或频道的](channel.md)。 

在包含 **一** 个或多个提及的 chatMessage 对象中，消息正文 **内容** 属性表示 HTML 形式的聊天消息。 它将每 **提及的提及文本** 包包在 HTML 元素内 `at` ，并 `id` 具有对应于提及 id 属性 **（Property）** 的属性 （Attribute）。

例如，一条聊天消息包含两个提及文字，分说明文字分为"Megan"和"Alex"。 它的 **正文** 内容属性 `at` 指定这两个提及的元素，如下所示：

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

在 content **属性中** ，第一个提及具有 HTML `id` 特性 0。 此属性对应于**chatMessageMention**的第一个实例的**id**属性，也是 0。

第二次提及具有 `id` 1 特性，它与第二个实例的 **id** 属性相匹配，即 1。

有关该示例的更全上下文，请参阅["列表频道消息回复"。](../api/channel-list-messagereplies.md#example)

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|Int32|指定 chatMessage 中提及的实体 **的索引**。 匹配邮件正文中相应标记中的 {index} `<at id="{index}">` 值。|
|mentionText|string|用于表示提及的字符串。 例如，用户的显示名称组名称。|
|提及|[identitySet](identityset.md)|实体的 (提及的用户、应用程序) 团队或频道。  如果是已有空的频道或 @mentioned团队，则 IdentitySet 包含 **为** 团队/频道提供 ID 的对话属性和一个 **conversationIdentityType** 属性，代表团队或频道。|


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
  "mentioned": {"@odata.type": "microsoft.graph.identitySet"}
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
