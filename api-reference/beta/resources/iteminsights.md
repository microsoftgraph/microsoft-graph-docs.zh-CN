---
title: itemInsights 资源类型
description: 用户与项目之间的关系，例如使用高级分析和机器学习技术计算得出的OneDrive for Business文档。 例如，你可以标识与用户有关的 OneDrive for Business 文档趋势。
author: simonhult
ms.localizationpriority: high
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 74452522b77e240c398c80a4dc8bec9c377efb09
ms.sourcegitcommit: ddeee0eec277df06d9e635e5b5c257d14c856273
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2021
ms.locfileid: "60780924"
---
# <a name="iteminsights-resource-type"></a>itemInsights 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用户与项目之间的关系，例如使用高级分析和机器学习技术计算得出的OneDrive for Business文档。 例如，你可以标识与用户有关的 OneDrive for Business 文档趋势。 派生自 [officeGraphInsights](officegraphinsights.md)。

Insights 由以下 API 返回：

- [趋势](insights-trending.md) - 返回与用户有关的 OneDrive for Business 和 SharePoint 网站趋势文档。
- [Used](insights-used.md) - 返回用户查看和修改过的文档。 包括用户在 OneDrive for Business 和 SharePoint 中使用的文档。
- [Shared](insights-shared.md) - 返回与用户共享的文档。 可作为电子邮件附件或电子邮件中发送的 OneDrive for Business 链接的文档。

返回的每个 insight 均为 `resourceVisualization` 和 `resourceReference` 复杂值类型 (CVT)。 resourceVisualization CVT 包含诸如 `title` 和 `previewImageUrl` 之类的属性。 Microsoft 使用可视化属性来渲染 Office Delve 等体验中的文件。

### <a name="limiting-item-insights"></a>限制项目见解

更新 [insightsSettings](insightssettings.md) 以禁用特定 Azure AD 组或整个组织的项目见解。 有关详细信息，请参阅[自定义见解隐私](/graph/insights-customize-item-insights-privacy)。

## <a name="properties"></a>属性

无。

## <a name="relationships"></a>关系

| 关系      | 类型          | 说明  |
| ------------- |---------------| -------------|
| 趋势      | [trending](insights-trending.md) 集合       | 用于标识与用户趋势文档的计算关系。 趋势文档是根据用户最近的人际网络活动来计算的，包括存储在 OneDrive for Business 和 SharePoint 的文件。 趋势见解帮助用户发现可能有用的内容，这些内容用户有权访问，但之前从未看过。|
| 使用的内容      | [usedInsight](insights-used.md) 集合        | 用于标识用户查看和修改的最新文档的计算关系，包括按使用时间排序的 OneDrive for Business 和 SharePoint 文档。|
| shared        | [sharedInsight](insights-shared.md) 集合        | 用于识别与或用户共享的文档的计算关系，包括电子邮件和会议中的文件附件，以及在电子邮件、会议和 Teams 对话中找到的 OneDrive for business 和 SharePoint 文件的 URL 和参考附件。按共享时间排序。|


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty":"id",
  "baseType":"microsoft.graph.officeGraphInsights",
  "optionalProperties": [
    "trending",
    "used",
    "shared"
  ],
  "@odata.type": "microsoft.graph.itemInsights"
}-->

```json
{
  "id": "string",
  "trending": [ { "@odata.type": "microsoft.graph.trending" } ],
  "used": [ { "@odata.type": "microsoft.graph.used" } ],
  "shared": [ { "@odata.type": "microsoft.graph.shared" } ]
}
```


