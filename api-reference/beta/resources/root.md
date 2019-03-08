---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 方根
localization_priority: Normal
ms.openlocfilehash: 8c320a34d22af5fc73a1c5d8c96dce14e176946f
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482369"
---
# <a name="root-resource-type"></a><span data-ttu-id="f46d2-102">根资源类型</span><span class="sxs-lookup"><span data-stu-id="f46d2-102">Root resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f46d2-103">**根** Facet 指示对象是它的层次结构中最顶层的对象。</span><span class="sxs-lookup"><span data-stu-id="f46d2-103">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="f46d2-104">若此 Facet 有值（非 null），表明对象是根。</span><span class="sxs-lookup"><span data-stu-id="f46d2-104">The presence (non-null) of the facet value indicates that the object is the root.</span></span>
<span data-ttu-id="f46d2-105">若值为 null（或缺失），表明对象不是根。</span><span class="sxs-lookup"><span data-stu-id="f46d2-105">A null (or missing) value indicates the object is not the root.</span></span>

<span data-ttu-id="f46d2-106">**注意**：尽管此 Facet 暂为空，但在今后推出的 API 版本中将在此 Facet 中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="f46d2-106">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f46d2-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f46d2-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="f46d2-108">属性</span><span class="sxs-lookup"><span data-stu-id="f46d2-108">Properties</span></span>

<span data-ttu-id="f46d2-109">**根**资源没有属性。</span><span class="sxs-lookup"><span data-stu-id="f46d2-109">The **Root** resource has no properties.</span></span>


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
