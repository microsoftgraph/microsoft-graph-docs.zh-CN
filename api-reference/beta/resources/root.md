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
# <a name="root-resource-type"></a><span data-ttu-id="f0d97-102">根资源类型</span><span class="sxs-lookup"><span data-stu-id="f0d97-102">Root resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f0d97-103">**根** Facet 指示对象是它的层次结构中最顶层的对象。</span><span class="sxs-lookup"><span data-stu-id="f0d97-103">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="f0d97-104">若此 Facet 有值（非 null），表明对象是根。</span><span class="sxs-lookup"><span data-stu-id="f0d97-104">The presence (non-null) of the facet value indicates that the object is the root.</span></span>
<span data-ttu-id="f0d97-105">若值为 null（或缺失），表明对象不是根。</span><span class="sxs-lookup"><span data-stu-id="f0d97-105">A null (or missing) value indicates the object is not the root.</span></span>

<span data-ttu-id="f0d97-106">**注意**：尽管此 Facet 暂为空，但在今后推出的 API 版本中将在此 Facet 中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="f0d97-106">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f0d97-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0d97-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="f0d97-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0d97-108">Properties</span></span>

<span data-ttu-id="f0d97-109">**根**资源没有属性。</span><span class="sxs-lookup"><span data-stu-id="f0d97-109">The **Root** resource has no properties.</span></span>


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
