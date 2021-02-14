---
author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: UploadSession 资源提供有关如何将大文件上载到 OneDrive、OneDrive for Business 或 SharePoint 文档库或作为 Outlook 事件和邮件对象的文件附件的信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0104b9349427b07ffef570d66b98720155bd7728
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239469"
---
# <a name="uploadsession-resource-type"></a>uploadSession 资源类型

命名空间：microsoft.graph

**uploadSession** 资源提供有关如何将大文件上载到 OneDrive、OneDrive for Business 或 SharePoint 文档库，或以附件方式 [上载到](event.md)Outlook 事件和 [邮件](message.md)项目的信息。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession"
}-->

```json
{
  "uploadUrl": "https://sn3302.up.1drv.com/up/fe6987415ace7X4e1eF866337",
  "expirationDateTime": "2015-01-29T09:21:55.523Z",
  "nextExpectedRanges": ["0-"]
}
```

## <a name="properties"></a>属性


| 属性       | 类型              |说明
|:-------------------|:------------------|:------------------------------------
| expirationDateTime | DateTimeOffset    | 以 UTC 表示的上载会话过期的日期和时间。在此过期时间之前必须上载完整的文件文件。
| nextExpectedRanges | String collection | 字节范围集合，文件服务器缺失。 这些区域索引均从零开始，格式为“开始-结束”（例如，“0-26”指示该文件的前 27 个字节)。 当将文件作为 Outlook 附件而不是范围集合上载时，此属性始终指示单个值"{start}"，即文件中应开始下一次上载的位置。
| uploadUrl          | String            | 接受文件字节范围的 PUT 请求的 URL 端点。

## <a name="see-also"></a>另请参阅

- [将大文件作为附件附加到 Outlook 邮件和事件 ](/graph/outlook-large-attachments)
- [通过上传会话上传大文件](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->

