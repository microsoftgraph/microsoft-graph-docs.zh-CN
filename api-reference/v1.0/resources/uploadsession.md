---
author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
ms.localizationpriority: medium
description: UploadSession 资源提供有关如何将大文件上载到 OneDrive、OneDrive for Business 或 SharePoint 文档库的信息，或作为 Outlook 事件和邮件对象的文件附件。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 056f3f520e5b66875fd67b01b581eeaa3caafcb2
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59006898"
---
# <a name="uploadsession-resource-type"></a>uploadSession 资源类型

命名空间：microsoft.graph

**uploadSession** 资源提供有关如何将大文件上载到 OneDrive、OneDrive for Business 或 SharePoint 文档库，或将 Outlook [事件](event.md)和邮件项目作为附件上载的信息。 [](message.md)

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
| nextExpectedRanges | String collection | 字节范围集合，文件服务器缺失。 这些区域索引均从零开始，格式为“开始-结束”（例如，“0-26”指示该文件的前 27 个字节)。 以附件Outlook文件（而不是范围集合）上载文件时，此属性始终指示单个值"{start}"，即文件中下一次上传应开始的位置。
| uploadUrl          | String            | 接受文件字节范围的 PUT 请求的 URL 端点。

## <a name="see-also"></a>另请参阅

- [将大文件附加到Outlook和事件作为附件](/graph/outlook-large-attachments)
- [通过上传会话上传大文件](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->

