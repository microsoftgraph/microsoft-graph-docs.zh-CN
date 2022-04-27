---
title: chatMessageAttachment 资源类型
description: 表示聊天消息实体的附件。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: microsoft-teams
author: RamjotSingh
ms.openlocfilehash: caf7d1693395d9272a8999910dcaa29a9bef11da
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65060756"
---
# <a name="chatmessageattachment-resource-type"></a>chatMessageAttachment 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示聊天消息实体的附件。

作为 [chatMessage](chatmessage.md) 实体的一部分，作为 [Get 频道消息](../api/channel-list-messages.md) API 的一部分返回类型的`chatMessageAttachment`实体。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string| 只读。 附件的唯一 ID。|
|contentType| string | 内容附件的媒体类型。 它可以具有以下值： <br><ul><li>`reference`：附件是指向另一个文件的链接。 使用指向对象的链接填充 contentURL。</li><li>Bot Framework 附[件对象](/azure/bot-service/rest-api/bot-framework-rest-connector-api-reference?#attachment-object)支持的任何 contentTypes</li><li>`application/vnd.microsoft.card.codesnippet`：代码片段。 </li><li>`application/vnd.microsoft.card.announcement`：公告标头。 </li>|
|contentUrl|string|附件内容的 URL。 支持的协议：http、https、文件和数据。|
|content|string|附件的内容。 如果附件是 [富卡](/microsoftteams/platform/task-modules-and-cards/cards/cards-reference)，请将属性设置为富卡对象。 此属性和 contentUrl 互斥。|
|name|string|附件的名称。|
|teamsAppId| string |与附件关联的Teams应用的 ID。 该属性专门用于将Teams消息卡属性到指定的应用。|
|thumbnailUrl| string |如果通道支持使用另一种形式较小的内容或 contentUrl，则可以使用该缩略图图像的 URL。 例如，如果将 contentType 设置为 application/word 并将 contentUrl 设置为 Word 文档的位置，则可能包含表示文档的缩略图。 通道可以显示缩略图而不是文档。 当用户单击图像时，通道将打开文档。|


## <a name="json-representation"></a>JSON 表示形式
 下面是资源的 JSON 表示形式

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "thumbnailUrl",
    "content",
    "contentUrl",
    "teamsAppId"
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
  "teamsAppId": "string",
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


