---
title: officeGraphInsights 资源类型
description: Insights 是使用高级分析和机器学习技术计算的关系。 例如，你可以标识与用户有关的 OneDrive for Business 文档趋势。
author: simonhult
ms.localizationpriority: high
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: ba7d88446850ddeddbd1f0b46995f4c363aa1e6d
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084207"
---
# <a name="officegraphinsights-resource-type"></a>officeGraphInsights 资源类型

命名空间：microsoft.graph

Insights 是使用高级分析和机器学习技术计算的关系。 例如，你可以标识与用户有关的 OneDrive for Business 文档趋势。

Insights 由以下 API 返回：

- [趋势](insights-trending.md) - 返回与用户有关的 OneDrive for Business 和 SharePoint 网站趋势文档。
- [使用](insights-used.md) - 返回用户查看或修改过的文档。 包括用户在 OneDrive for Business 和 SharePoint 中使用的文档。
- [分享](insights-shared.md) - 返回与用户共享或由用户共享的文档。 文档可以作为 OneDrive for Business 和 SharePoint 的 URL、文件附件、参考附件共享，这些可以在 Outlook 邮件和会议中找到。

每个见解都返回 **resourceVisualization** 和 **resourceReference** 复杂值类型 (CVT)。 **resourceVisualization** CVT 包含诸如 **title** 和 **previewImageUrl** 之类的属性。 Microsoft 使用可视化属性来渲染 Office Delve 等体验中的文件。

## <a name="relationships"></a>关系

| 关系      | 类型          | 说明  |
| ------------- |---------------| -------------|
| 趋势      | [trending](insights-trending.md) 集合       | 用于标识与用户趋势文档的计算关系。 趋势文档是根据用户最近的人际网络活动来计算的，包括存储在 OneDrive for Business 和 SharePoint 的文件。 趋势见解帮助用户发现可能有用的内容，这些内容用户有权访问，但之前从未看过。|
| 使用的内容      | [usedInsight](insights-used.md) 集合        | 用于标识用户查看或修改的最新文档的计算关系，包括按使用时间排序的 OneDrive for Business 和 SharePoint 文档。|
| shared        | [sharedInsight](insights-shared.md) 集合        | 标识与用户共享或由用户共享的文档的计算关系。这包括 URL、文件附件以及在 Outlook 邮件和会议中找到的 OneDrive for Business 和 SharePoint 文件的引用附件。还包括 URL 和 Teams 对话的引用附件。按共享的新近顺序排序。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "baseType":"microsoft.graph.entity",
  "optionalProperties": [
    "trending",
    "used",
    "shared"
  ],
  "@odata.type": "microsoft.graph.officeGraphInsights"
}-->

```json
{
  "id": "string",
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```

