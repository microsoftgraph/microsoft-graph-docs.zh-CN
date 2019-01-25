---
title: resourceVisualization 资源类型
description: 包含属性的见解复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ec1619d07d0f31bf8325c25b161084f505b3ee
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526758"
---
# <a name="resourcevisualization-resource-type"></a>resourceVisualization 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含属性的[见解](insights.md)复杂类型。

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
| title                 | String        | 项目的标题文本。               |
| type              | String        | 项目的媒体类型。 可用于根据特定类型的特定文件筛选。 请参阅以下支持的类型。 |
| MediaType             | String        | 项目的媒体类型。 可用于筛选文件根据支持 IANA 媒体 Mime 类型为特定类型。 请注意，不是所有媒体 Mime 类型都受都支持。 |
| PreviewImageUrl       | String        | 导致项目的预览图像 URL。 |
| previewText           | String        | 预览文本项。 |
| containerWebUrl       | String        | 前导到在其中存储项目的文件夹路径。 |
| containerDisplayName  | String        | 描述项目的存储位置的字符串。 例如，SharePoint 网站或标识的 OneDrive 存储项目所有者的用户名称的名称。  |
| ContainerType         | String | 可用于筛选按在其中存储文件的容器的类型。 如 Site 或 OneDriveBusiness。       |

## <a name="type-property-values"></a>类型属性值
-   PowerPoint
-   Word
-   Excel
-   PDF
-   OneNote
-   OneNotePage
-   InfoPath
-   Visio
-   Publisher
-   项目
-   Access
-   邮件
-   *.csv
-   存档
-   Xps
-   音频
-   视频
-   图像
-   Web
-   文本
-   Xml
-   文章
-   ExternalContent
-   Folder
-   Other

示例查询：`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>containerType 属性值
受支持的类型从其[洞察](insights.md)返回文件的容器可能因用。 例如，仅[共享](insights-shared.md)洞察返回文件 '收存箱、 框中，和 GDrive。

-   OneDriveBusiness
-   Site
-   邮件
-   收存箱
-   盒状
-   GDrive

示例查询：`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/insights-resourcevisualization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
