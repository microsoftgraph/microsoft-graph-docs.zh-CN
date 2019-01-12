---
title: 见解资源类型
description: 见解是计算使用高级分析功能和机学习技术的关系。 例如，可以确定趋势周围用户的 OneDrive 文档。
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 38f7afb40c1618a8a7cf9d585c99633e2bb8d940
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938312"
---
# <a name="insights-resource-type"></a>见解资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

见解是计算使用高级分析功能和机学习技术的关系。 例如，可以确定趋势周围用户的 OneDrive 文档。

见解会返回以下 Api:

- [趋势](insights-trending.md)-返回文档从 OneDrive 和趋势周围用户的 SharePoint 网站。
- [用于](insights-used.md)-返回文档查看和修改的用户。 包含用户使用的文档中的 OneDrive for Business，SharePoint 中，打开作为电子邮件附件和为如框、 收存箱和 Google 驱动器的源中的链接附件。
- [共享](insights-shared.md)-返回与用户共享的文档。 文档可以共享作为电子邮件附件或 OneDrive for Business 链接中发送电子邮件。

每个洞察返回了`resourceVisualization`和`resourceReference`复杂值类型 (CVT)。 ResourceVisualization CVT 包含属性，如`title`和`previewImageUrl`。 Microsoft 使用可视化属性来呈现像 Office 深入体验中的文件。

## <a name="relationships"></a>Relationships

| 关系      | 类型          | 说明  |
| ------------- |---------------| -------------|
| 趋势分析      | [趋势](insights-trending.md)集合       | 确定趋势文档的关系计算。 可以存储趋势文档，在 OneDrive 或 SharePoint 网站中。   |
| used      | [用于](insights-used.md)集合       | 计算确定文档查看和修改的用户的关系。 包含用户使用的文档中的 OneDrive for Business，SharePoint 中，打开作为电子邮件附件和为如框、 收存箱和 Google 驱动器的源中的链接附件。  |
| shared        | [共享](insights-shared.md)集合       | 确定与用户共享的文档的关系计算。 文档可以共享作为电子邮件附件或 OneDrive for Business 链接中发送电子邮件。   |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
```json
{
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```
