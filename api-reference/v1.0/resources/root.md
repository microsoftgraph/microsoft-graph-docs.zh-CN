---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Root
ms.openlocfilehash: 36d283792e25d5718b66190a5289ae4a7ff3d992
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="root-resource-type"></a><span data-ttu-id="0015e-102">Root 资源类型</span><span class="sxs-lookup"><span data-stu-id="0015e-102">Root resource type</span></span>

<span data-ttu-id="0015e-103">**Root** Facet 指示对象是它的层次结构中最顶层的对象。</span><span class="sxs-lookup"><span data-stu-id="0015e-103">The **Root** facet indicates that an object is the top-most one in its hierarchy.</span></span>
<span data-ttu-id="0015e-104">如果存在 Facet 值（非 null），则表明对象是根。</span><span class="sxs-lookup"><span data-stu-id="0015e-104">The presence (non-null) of the facet value indicates that the driveItem is the root.</span></span>
<span data-ttu-id="0015e-105">如果值为 null（或缺失），则表明对象不是根。</span><span class="sxs-lookup"><span data-stu-id="0015e-105">A null (or missing) value indicates the driveItem is not the root..</span></span>

<span data-ttu-id="0015e-106">**注意**：尽管此 Facet 暂为空，但在今后推出的 API 版本中将在此 Facet 中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="0015e-106">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0015e-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0015e-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.root" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="0015e-108">属性</span><span class="sxs-lookup"><span data-stu-id="0015e-108">Properties</span></span>

<span data-ttu-id="0015e-109">**根**资源没有属性。</span><span class="sxs-lookup"><span data-stu-id="0015e-109">The **Root** resource has no properties.</span></span>


<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/Root"
} -->
