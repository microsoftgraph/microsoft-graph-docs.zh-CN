---
title: chatMessageAttachment 资源类型
description: 表示聊天消息实体的附件。
localization_priority: Normal
ms.openlocfilehash: 83574a7dbbb35f9c8b95474fac1154154f413470
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805556"
---
# <a name="chatmessageattachment-resource-type"></a>chatMessageAttachment 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

表示聊天消息实体的附件。

实体类型的`chatMessageAttachment`返回作为一部分[获取通道消息](../api/channel-list-messages.md)API，作为[chatMessage](chatmessage.md)实体的一部分。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|ID|string| 只读。 附件的唯一 id|
|contentType| string | 媒体类型的内容的附件。 它可以具有以下值： <br><ul><li>参考： 附件是到另一个文件的链接。 填充与对对象链接 contentURL<br></li><li>文件： 原始文件附件。 填充具有中数据的文件的 base64 编码的 contenturl 字段： 格式<br></li><li>图像 /: 与指定的图像的类型图像类型： 图像/png、 image/jpeg 图像/gif。 填充具有中数据的文件的 base64 编码的 contentUrl 字段： 格式<br></li><li>视频 /: 视频指定的格式的类型。 示例： 视频/mp4 （英文)。 填充具有中数据的文件的 base64 编码的 contentUrl 字段： 格式<br></li><li>音频 /: 具有指定的格式的音频类型。 示例： 音频/wmw。 填充具有中数据的文件的 base64 编码的 contentUrl 字段： 格式<br></li><li>应用程序/名片类型： 富卡片与指定的确切卡格式的卡片类型使用的附件类型。 设置与卡片的 json 格式的内容。 支持的名片类型的值包括：<br><ul><li>application/vnd.microsoft.card.adaptive： 可包含文本、 语音、 图像、 按钮和输入的字段的任意组合的丰富卡片。 设置对，AdaptiveCard 对象的内容的属性。</li><li>application/vnd.microsoft.card.animation： 播放动画的丰富卡片。 设置为 AnimationCardobject 的内容的属性。</li><li>application/vnd.microsoft.card.audio： 播放音频文件的丰富卡片。 设置为 AudioCard 对象的内容的属性。</li><li>application/vnd.microsoft.card.video： 播放视频的丰富卡片。 设置为视频卡的详细对象的内容的属性。</li><li>application/vnd.microsoft.card.hero： 生卡片。 内容属性设置为 HeroCard 对象。</li><li>application/vnd.microsoft.card.thumbnail： 的缩略图卡片。 内容属性设置为 ThumbnailCard 对象。</li><li>application/vnd.microsoft.com.card.receipt： 回执卡片。 内容属性设置为 ReceiptCard 对象。</li><li>application/vnd.microsoft.com.card.signin： 用户登录卡片。 内容属性设置为 SignInCard 对象。</ul></ul>|
|contentUrl|string|内容的附件的 URL。 支持的协议： http、 https、 文件和数据|
|content|string|附件的内容。 如果附件是丰富卡，设置对丰富卡对象的属性。 此属性和 contentUrl 都是互斥的|
|name|string|附件的名称|
|thumbnailUrl| string |URL 如果它支持使用替代、 较小的内容或 contentUrl 窗体，可以使用该频道的缩略图。 例如，如果您将 contentType 设置为应用程序/word，并将 contentUrl 设置为 Word 文档的位置，则可能包括表示的文档的缩略图。 该频道可以显示而不是文档的缩略图图像。 当用户单击图像时，通道将打开的文档。|

## <a name="json-representation"></a>JSON 表示形式
 以下是资源的 JSON 表示形式

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
<!-- {
  "type": "#page.annotation",
  "description": "chat attachment resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
