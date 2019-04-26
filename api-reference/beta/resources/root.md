---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 方根
localization_priority: Normal
ms.openlocfilehash: 83211263f4ba7998ea9e1863756f5aba7b6ff070
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343505"
---
# <a name="root-resource-type"></a><span data-ttu-id="6ce71-102">根资源类型</span><span class="sxs-lookup"><span data-stu-id="6ce71-102">Root resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ce71-103">**根** Facet 指示对象是它的层次结构中最顶层的对象。</span><span class="sxs-lookup"><span data-stu-id="6ce71-103">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="6ce71-104">若此 Facet 有值（非 null），表明对象是根。</span><span class="sxs-lookup"><span data-stu-id="6ce71-104">The presence (non-null) of the facet value indicates that the object is the root.</span></span>
<span data-ttu-id="6ce71-105">若值为 null（或缺失），表明对象不是根。</span><span class="sxs-lookup"><span data-stu-id="6ce71-105">A null (or missing) value indicates the object is not the root.</span></span>

<span data-ttu-id="6ce71-106">**注意**：尽管此 Facet 暂为空，但在今后推出的 API 版本中将在此 Facet 中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="6ce71-106">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ce71-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6ce71-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="6ce71-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ce71-108">Properties</span></span>

<span data-ttu-id="6ce71-109">**根**资源没有属性。</span><span class="sxs-lookup"><span data-stu-id="6ce71-109">The **Root** resource has no properties.</span></span>


<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root",
  "suppressions": []
}
-->
