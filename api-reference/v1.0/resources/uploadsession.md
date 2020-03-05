---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
description: UploadSession 资源提供了有关如何将大文件上传到 OneDrive、OneDrive for Business 或 SharePoint 文档库的信息。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3537a59da65499e67283d8a0640e5392c65edce1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446784"
---
# <a name="uploadsession-resource"></a>UploadSession 资源

命名空间： microsoft. graph

**UploadSession** 资源提供了有关如何将大文件上传到 OneDrive、OneDrive for Business 或 SharePoint 文档库的信息。

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
| nextExpectedRanges | String collection | 字节范围集合，文件服务器缺失。这些区域索引均从零开始，格式为“开始-结束”（例如，“0-26”指示该文件的前 27 个字节)。
| uploadUrl          | String            | 接受文件字节范围的 PUT 请求的 URL 端点。

## <a name="see-also"></a>另请参阅

- [通过上传会话上传大文件](../api/driveitem-createuploadsession.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession"
} -->
