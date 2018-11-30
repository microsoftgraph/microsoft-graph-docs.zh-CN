---
title: resourceVisualization 资源类型
description: 包含属性的见解复杂类型。
ms.openlocfilehash: 3ed61a8547e072938fc073d90f2592baf4c08fba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046537"
---
# <a name="resourcevisualization-resource-type"></a>resourceVisualization 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

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
| title                 | 字符串        | 项目的标题文本。               |
| type              | 字符串        | 项目的媒体类型。 可用于根据特定类型的特定文件筛选。 请参阅以下支持的类型。 |
| 媒体类型             | 字符串        | 项目的媒体类型。 可用于筛选文件根据支持 IANA 媒体 Mime 类型为特定类型。 请注意，不是所有媒体 Mime 类型都受都支持。 |
| previewImageUrl       | 字符串        | 导致项目的预览图像 URL。 |
| previewText           | 字符串        | 预览文本项。 |
| containerWebUrl       | 字符串        | 前导到在其中存储项目的文件夹路径。 |
| containerDisplayName  | 字符串        | 描述项目的存储位置的字符串。 例如，SharePoint 网站或标识的 OneDrive 存储项目所有者的用户名称的名称。  |
| containerType         | 字符串 | 可用于筛选按在其中存储文件的容器的类型。 如 Site 或 OneDriveBusiness。       |

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
-   文章
-   ExternalContent
-   文件夹
-   其他

示例查询：`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/Type eq 'PowerPoint'`

## <a name="containertype-property-values"></a>containerType 属性值
受支持的类型从其[洞察](insights.md)返回文件的容器可能因用。 例如，仅[共享](insights-shared.md)洞察返回文件 '收存箱、 框中，和 GDrive。

-   OneDriveBusiness
-   网站
-   邮件
-   收存箱
-   盒状
-   GDrive

示例查询：`https://graph.microsoft.com/beta/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`