---
author: JeremyKelley
description: 表示用于将大型文件上载到 OneDrive、OneDrive for Business 或 SharePoint 文档库，或作为 Outlook 事件和邮件对象的文件附件的迭代过程的信息。
title: uploadSession 资源类型
localization_priority: Normal
doc_type: resourcePageType
ms.prod: non-product-specific
ms.openlocfilehash: 9dd76265e08cc377aba295679a35f33f2256b3b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003442"
---
# <a name="uploadsession-resource-type"></a>uploadSession 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示用于将大型文件上传到 OneDrive、OneDrive for Business 或 SharePoint 文档库，或将 Outlook [事件](event.md) 和 [邮件](message.md) 项作为附件的迭代过程的信息。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [ "uploadUrl", "nextExpectedRanges" ],
  "@odata.type": "microsoft.graph.uploadSession",
  "baseType": null
}-->

```json
{
  "uploadUrl": "String",
  "expirationDateTime": "String (timestamp)",
  "nextExpectedRanges": ["String"]
}
```

## <a name="properties"></a>属性


| 属性       | 类型              |说明
|:-------------------|:------------------|:------------------------------------
| expirationDateTime | DateTimeOffset    | 以 UTC 表示的上载会话过期的日期和时间。在此过期时间之前必须上载完整的文件文件。
| nextExpectedRanges | String collection | 将文件上载到文档库时，这是文件的服务器缺少的字节范围的集合。 这些区域的索引为零，格式为 "{start}-{end}" (例如，"0-26" 表示文件) 的前27个字节。 将文件作为 Outlook 附件（而不是区域集合）上载时，此属性始终指示单个值 "{start}"，即文件中应开始下一次上载的位置。
| uploadUrl          | String            | 接受文件字节范围的 PUT 请求的 URL 端点。

## <a name="see-also"></a>另请参阅

- [将大型文件作为附件附加到 Outlook 邮件和事件 ](/graph/outlook-large-attachments)
- [通过上传会话上传大文件](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession",
  "suppressions": []
}
-->


