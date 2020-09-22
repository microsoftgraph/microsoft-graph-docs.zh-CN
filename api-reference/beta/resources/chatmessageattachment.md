---
title: chatMessageAttachment 资源类型
description: 表示聊天消息实体的附件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: clearab
ms.openlocfilehash: 2c343d3449365d34c0bda0fd35b58e029d89711f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48064309"
---
# <a name="chatmessageattachment-resource-type"></a>chatMessageAttachment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示聊天消息实体的附件。

类型的实体作为 `chatMessageAttachment` [Get 信道消息](../api/channel-list-messages.md) API 的一部分返回，作为 [了 chatmessage](chatmessage.md) 实体的一部分。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string| 只读。 附件的唯一 id。|
|contentType| string | 内容附件的媒体类型。 它可以具有以下值： <br><ul><li>`reference`：附件是指向其他文件的链接。 使用指向对象的链接填充 contentURL。</li><li>Bot 框架的[附件对象](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?view=azure-bot-service-4.0#attachment-object)支持的任何 contentTypes</li><li>`application/vnd.microsoft.card.codesnippet`：代码段。 </li><li>`application/vnd.microsoft.card.announcement`：通知标头。 </li>|
|contentUrl|string|附件内容的 URL。 支持的协议： http、https、文件和数据。|
|content|string|附件的内容。 如果附件是一个 [丰富的卡片](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference)，请将该属性设置为富卡片对象。 此属性和 contentUrl 相互排斥。|
|name|string|附件的名称。|
|thumbnailUrl| string |如果通道支持使用替代的较小的内容或 contentUrl 的缩略图图像的 URL。 例如，如果将 contentType 设置为 application/word 并将 contentUrl 设置为 Word 文档的位置，则可以包含表示该文档的缩略图图像。 频道可以显示缩略图图像而不是文档。 当用户单击图像时，通道将打开文档。|

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


