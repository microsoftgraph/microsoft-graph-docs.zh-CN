---
title: resourceVisualization 资源类型
description: 包含见解的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550733"
---
# <a name="resourcevisualization-resource-type"></a>resourceVisualization 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含[见解](insights.md)的属性的复杂类型。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

```json
{
  "title": "string",
  "type"  : "string",
  "mediaType": "string",
  "previewImageUrl": "string",
  "previewText": "string",
  "containerWebUrl": "string",
  "containerDisplayName": "string",
  "containerType": "string"
}
```

## <a name="properties"></a>属性

| 属性              | 类型          | 说明  |
| -------------         |---------------| -------------|
| title                 | 字符串        | 项目的标题文本。               |
| 类型              | String        | 项目的媒体类型。 可用于根据特定类型筛选特定文件。 请参阅以下支持的类型。 |
| 群组             | String        | 项目的媒体类型。 可用于根据受支持的 IANA 媒体 Mime 类型筛选特定类型的文件。 请注意, 并非所有媒体 Mime 类型都受支持。 |
| previewImageUrl       | String        | 指向项目的预览图像的 URL。 |
| previewText           | String        | 项目的预览文本。 |
| containerWebUrl       | String        | 指向存储项目的文件夹的路径。 |
| containerDisplayName  | String        | 一个描述项目存储位置的字符串。 例如, SharePoint 网站的名称或标识 OneDrive 的所有者存储项目的用户名。  |
| containerType         | String | 可用于按存储文件的容器的类型进行筛选。 如 Site 或 OneDriveBusiness。       |

## <a name="type-property-values"></a>类型属性值
-   PowerPoint
-   Word
-   Excel
-   Pdf
-   OneNote
-   OneNotePage
-   InfoPath
-   Visio
-   Publisher
-   Project
-   Access
-   邮件
-   Csv
-   存档
-   Xps
-   音频
-   视频
-   图像
-   Web
-   Text
-   Xml
-   Story
-   ExternalContent
-   Folder
-   其他

示例查询:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>containerType 属性值
根据[真知灼见](insights.md)返回文件的容器, 支持的类型会有所不同。 例如, 只有[共享](insights-shared.md)的洞察力才会从 "收存箱"、"Box" 和 "GDrive" 返回文件。

-   OneDriveBusiness
-   Site
-   邮件
-   箱
-   Box
-   GDrive

示例查询:`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
