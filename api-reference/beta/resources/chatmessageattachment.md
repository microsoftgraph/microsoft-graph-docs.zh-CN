---
title: chatMessageAttachment 资源类型
description: 表示聊天消息实体的附件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-teams
author: RamjotSingh
ms.openlocfilehash: b4660e92643d868fbd09c693187a486fc3937584
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582569"
---
# <a name="chatmessageattachment-resource-type"></a>chatMessageAttachment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示聊天消息实体的附件。

类型实体作为 `chatMessageAttachment` [chatMessage](chatmessage.md)实体的一部分作为[获取](../api/channel-list-messages.md)频道消息 API 的一部分返回。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string| 只读。 附件的唯一 ID。|
|contentType| string | 内容附件的媒体类型。 它可以具有以下值： <br><ul><li>`reference`：Attachment 是指向其他文件的链接。 使用指向对象的链接填充 contentURL。</li><li>Bot Framework 的 Attachment 对象支持的任何 [contentType](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?#attachment-object)</li><li>`application/vnd.microsoft.card.codesnippet`：代码段。 </li><li>`application/vnd.microsoft.card.announcement`：通知标头。 </li>|
|contentUrl|string|附件内容的 URL。 支持的协议：http、https、文件和数据。|
|content|string|附件的内容。 如果附件是富 [卡片，](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference)将 属性设置为富卡片对象。 此属性和 contentUrl 相互排斥。|
|name|string|附件的名称。|
|thumbnailUrl| string |指向缩略图图像的 URL，如果频道支持使用其他较小格式的内容或 contentUrl，可以使用该图像。 例如，如果将 contentType 设置为 application/word，并且将 contentUrl 设置为 Word 文档的位置，则可能包含表示文档的缩略图图像。 通道可以显示缩略图图像而不是文档。 当用户单击该图像时，通道将打开文档。|

## <a name="json-representation"></a>JSON 表示形式
 下面是资源的 JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "thumbnailUrl",
    "content",
    "contentUrl"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.chatMessageAttachment"
}-->

```json
{
  "id": "string (identifier)",
  "contentType": "string",
  "contentUrl": "string",
  "content": "string",
  "name": "string",
  "thumbnailUrl": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


