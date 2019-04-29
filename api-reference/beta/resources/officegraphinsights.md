---
title: officeGraphInsights 资源类型
description: Insights 是使用高级分析和机器学习技术计算的关系。 例如，你可以标识与用户有关的 OneDrive 文档趋势。
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.openlocfilehash: 8a07cd10622886ad6e367d5311e750454e7bf90b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348588"
---
# <a name="officegraphinsights-resource-type"></a>officeGraphInsights 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Insights 是使用高级分析和机器学习技术计算的关系。 例如，你可以标识与用户有关的 OneDrive 文档趋势。

Insights 由以下 API 返回：

- [Trending](insights-trending.md) - 返回与用户有关的 OneDrive 和 SharePoint 网站趋势文档。
- [Used](insights-used.md) - 返回用户查看和修改过的文档。 包括在 OneDrive for Business 和 SharePoint 中使用的文档、以电子邮件附件打开的文档以及来自源（如 Box、DropBox 和 Google 云端硬盘）的链接附件文档。
- [Shared](insights-shared.md) - 返回与用户共享的文档。 可作为电子邮件附件或电子邮件中发送的 OneDrive for Business 链接的文档。

返回的每个 insight 均为 `resourceVisualization` 和 `resourceReference` 复杂值类型 (CVT)。 resourceVisualization CVT 包含诸如 `title` 和 `previewImageUrl` 之类的属性。 Microsoft 使用可视化属性来渲染 Office Delve 等体验中的文件。

## <a name="relationships"></a>关系

| 关系      | 类型          | 说明  |
| ------------- |---------------| -------------|
| 趋势      | [trending](insights-trending.md) 集合       | 用于标识趋势文档的计算关系。 趋势文档可以存储在 OneDrive 或 SharePoint 网站中。   |
| 使用的内容      | [usedInsight](insights-used.md) 集合        | 用于标识用户已查看和修改文档的计算关系。 包括在 OneDrive for Business 和 SharePoint 中使用的文档、以电子邮件附件打开的文档以及来自源（如 Box、DropBox 和 Google 云端硬盘）的链接附件文档。  |
| shared        | [sharedInsight](insights-shared.md) 集合        | 用于标识与用户共享的文档的计算关系。 可作为电子邮件附件或电子邮件中发送的 OneDrive for Business 链接的文档。   |

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
