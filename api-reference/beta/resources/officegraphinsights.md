---
title: officeGraphInsights 资源类型
description: 表示 itemInsights 的基本类型。 officeGraphInsights 向后兼容 insights API 的早期版本。 访问 insights API 时只能使用 itemInsights。
author: simonhult
ms.localizationpriority: high
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 308d35e19eaf1ac5454b33b030d2e9c0a7f7a416
ms.sourcegitcommit: c333953a9188b4cd4a9ab94cbe68871e8f3563e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58695915"
---
# <a name="officegraphinsights-resource-type"></a>officeGraphInsights 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 [itemInsights](iteminsights.md) 替代 **officeGraphInsights** 以访问 insights API。

**officeGraphInsights** 向后兼容 insights API 的早期版本。 它是 [itemInsights](iteminsights.md) 的基础类型。

Insights 是使用高级分析和机器学习技术计算的关系。 例如，你可以标识与用户有关的 OneDrive for Business 文档趋势。

Insights 由以下 API 返回：

- [趋势](insights-trending.md) - 返回与用户有关的 OneDrive for Business 和 SharePoint 网站趋势文档。
- [使用](insights-used.md) - 返回用户查看或修改过的文档。 包括用户在 OneDrive for Business 和 SharePoint 中使用的文档。
- [分享](insights-shared.md) - 返回与用户共享或由用户共享的文档。 文档可以作为 OneDrive for Business 和 SharePoint 的 URL、文件附件、参考附件共享，这些可以在 Outlook 邮件和会议中找到。

每个见解都返回 **resourceVisualization** 和 **resourceReference** 复杂值类型 (CVT)。 **resourceVisualization** CVT 包含诸如 **title** 和 **previewImageUrl** 之类的属性。 Microsoft 使用可视化属性来渲染 Office Delve 等体验中的文件。

## <a name="relationships"></a>关系

| 关系      | 类型          | 说明  |
| ------------- |---------------| -------------|
| 趋势      | [trending](insights-trending.md) 集合       | 从派生类型 [itemInsights](iteminsights.md) 访问此属性。|
| 使用的内容      | [usedInsight](insights-used.md) 集合        | 从派生类型 [itemInsights](iteminsights.md) 访问此属性。|
| shared        | [sharedInsight](insights-shared.md) 集合        | 从派生类型 [itemInsights](iteminsights.md) 访问此属性。|


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



