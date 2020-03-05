---
title: chatMessageAttachment 资源类型
description: 表示聊天消息实体的附件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 45058b5d3217072d5e70875574fdee9de7eb20a0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507710"
---
# <a name="chatmessageattachment-resource-type"></a>chatMessageAttachment 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示聊天消息实体的附件。

类型`chatMessageAttachment`的实体作为[Get 信道消息](../api/channel-list-messages.md)API 的一部分返回，作为[了 chatmessage](chatmessage.md)实体的一部分。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string| 只读。 附件的唯一 id。|
|contentType| string | 内容附件的媒体类型。 它可以具有以下值： <br><ul><li>"引用：附件" 是指向其他文件的链接。 使用指向对象的链接填充 contentURL。<br></li><li>文件： Raw 文件附件。 使用 data：格式的文件的 base64 编码填充 contenturl 字段。<br></li><li>image/：带有指定图像类型（如 image/png、image/jpeg、image/gif）的图像类型。 使用 data：格式的文件的 base64 编码填充 contentUrl 字段。<br></li><li>视频/：具有指定格式的视频类型。 Ex： video/.。 使用 data：格式的文件的 base64 编码填充 contentUrl 字段。<br></li><li>音频/：指定格式的音频类型。 Ex：音频/wmw。 使用 data：格式的文件的 base64 编码填充 contentUrl 字段。<br></li><li>应用程序/卡片类型：使用卡片类型指定要使用的确切卡片格式的富卡片附件类型。 使用该卡片的 json 格式设置内容。 卡片类型支持的值包括：<br><ul><li>应用程序/vnd.ms-excel：可包含文本、语音、图像、按钮和输入字段的任意组合的丰富卡片。 将 content 属性设置为一个自适应卡片对象。</li><li>应用程序/vnd.ms-excel：播放动画的富卡片。 将 content 属性设置为 AnimationCardobject。</li><li>vnd.ms-excel：一种播放音频文件的丰富卡片。 将 content 属性设置为 AudioCard 对象。</li><li>vnd.ms-excel：一种播放视频的丰富卡片。 将 content 属性设置为 VideoCard 对象。</li><li>应用程序/vnd.ms-excel：英雄卡片。 将 content 属性设置为 HeroCard 对象。</li><li>application/vnd.ms-excel：缩略图卡片。 将 content 属性设置为 ThumbnailCard 对象。</li><li>应用程序/vnd.ms-excel：一个收据卡。 将 content 属性设置为 ReceiptCard 对象。</li><li>应用程序/vnd.ms-excel：登录的用户的卡。 将 content 属性设置为 SignInCard 对象。</ul></ul>|
|contentUrl|string|附件内容的 URL。 支持的协议： http、https、文件和数据。|
|content|string|附件的内容。 如果附件是一个丰富的卡片，请将该属性设置为富卡片对象。 此属性和 contentUrl 相互排斥。|
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
