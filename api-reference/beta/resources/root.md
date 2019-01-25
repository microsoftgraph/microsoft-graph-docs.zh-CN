---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Root
localization_priority: Normal
ms.openlocfilehash: dda2de3e92128a9813f923d9acfef0eec94680e5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510300"
---
# <a name="root-resource-type"></a>根资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**根** Facet 指示对象是它的层次结构中最顶层的对象。
若此 Facet 有值（非 null），表明对象是根。
若值为 null（或缺失），表明对象不是根。

**注意**：尽管此 Facet 暂为空，但在今后推出的 API 版本中将在此 Facet 中填充其他属性。

## <a name="json-representation"></a>JSON 表示形式

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a>属性

**根**资源没有属性。


<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root",
  "suppressions": [
    "Error: /api-reference/beta/resources/root.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
