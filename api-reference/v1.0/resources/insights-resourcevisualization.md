---
title: resourceVisualization 资源类型
description: 包含见解的属性的复杂类型。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 39810868e779f9de62535e4b463f477f12739e85
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39845019"
---
# <a name="resourcevisualization-resource-type"></a>resourceVisualization 资源类型

包含[officeGraphInsights](officegraphinsights.md)的属性的复杂类型。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],  
  "@odata.type": "microsoft.graph.resourceVisualization"
}-->
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
| type              | 字符串        | 项目的媒体类型。 可用于根据特定类型筛选特定文件。 请参阅以下支持的类型。 |
| 群组             | String        | 项目的媒体类型。 可用于根据受支持的 IANA 媒体 Mime 类型筛选特定类型的文件。 请注意，并非所有媒体 Mime 类型都受支持。 |
| previewImageUrl       | String        | 指向项目的预览图像的 URL。 |
| previewText           | String        | 项目的预览文本。 |
| containerWebUrl       | String        | 指向存储项目的文件夹的路径。 |
| containerDisplayName  | String        | 一个描述项目存储位置的字符串。 例如，SharePoint 网站的名称或标识 OneDrive 的所有者存储项目的用户名。  |
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
-   项目
-   Access
-   邮件
-   Csv
-   存档
-   Xps
-   音频
-   视频
-   图像
-   Web
-   文本
-   Xml
-   Story
-   ExternalContent
-   Folder
-   Other

示例查询：`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>containerType 属性值
根据[officeGraphInsights](officegraphinsights.md)返回文件的容器，受支持的类型可能有所不同。 例如，仅[sharedInsight](insights-shared.md)真知灼见将从 "收存箱"、"Box" 和 "GDrive" 返回文件。

-   OneDriveBusiness
-   Site
-   邮件
-   箱
-   Box
-   GDrive

示例查询：`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`
