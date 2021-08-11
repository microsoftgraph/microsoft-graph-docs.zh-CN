---
title: resourceVisualization 资源类型
description: 包含属性的复杂Insights。
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: a8f5d97a41e28e103d6cf756bb08790deef8c1ee0fa4a44b40a363bc759cf8ae
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126569"
---
# <a name="resourcevisualization-resource-type"></a>resourceVisualization 资源类型

命名空间：microsoft.graph

包含 [officeGraphInsights 属性的复杂类型](officegraphinsights.md)。

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
| type              | String        | 项的媒体类型。 可用于根据特定类型筛选特定文件。 有关支持的类型，请参阅下文。 |
| mediaType             | String        | 项的媒体类型。 可用于基于支持的 IANA 媒体 Mime 类型筛选特定类型的文件。 请注意，并非所有媒体 Mime 类型都受支持。 |
| previewImageUrl       | String        | 指向项目的预览图像的 URL。 |
| previewText           | String        | 项的预览文本。 |
| containerWebUrl       | String        | 指向存储项目的文件夹的路径。 |
| containerDisplayName  | String        | 一个描述项存储位置的字符串。 例如，网站名称SharePoint或用于标识项目存储OneDrive所有者的用户名。  |
| containerType         | String | 可用于按存储文件的容器类型进行筛选。 例如 Site 或 OneDriveBusiness。       |

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
-   文本
-   Xml
-   Story
-   ExternalContent
-   Folder
- Spsite
-   其他

示例查询： `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

注意： `spsite` 可能需要按 `lastUsed/lastAccessedDateTime` desc 排序才能检索有效结果

## <a name="containertype-property-values"></a>containerType 属性值
支持的类型可能因 [officeGraphInsights](officegraphinsights.md) 返回文件的容器不同。 例如，仅 [sharedInsight](insights-shared.md) 见解从"DropBox"、"Box"和"GDrive"返回文件。

-   OneDriveBusiness
-   Site
-   邮件
-   DropBox
-   Box
-   GDrive

示例查询： `https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

