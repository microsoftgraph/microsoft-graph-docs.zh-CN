---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: UploadSession
localization_priority: Normal
ms.openlocfilehash: c5d15c380908f09ef292b7c5794046bad6e95ac8
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507948"
---
# <a name="uploadsession-resource"></a>UploadSession 资源

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

- 通过上传会话上传大文件

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "UploadSession is used to provide information about large file uploads.",
  "section": "documentation",
  "tocPath": "Resources/UploadSession",
  "suppressions": [
    "Error: /api-reference/beta/resources/uploadsession.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
