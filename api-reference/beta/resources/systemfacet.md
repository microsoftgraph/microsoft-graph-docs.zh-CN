---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: SystemFacet
localization_priority: Normal
ms.openlocfilehash: afafb69e9d887d2cb8d9537dd7ef9d3a712f3333
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528548"
---
# <a name="system-facet"></a><span data-ttu-id="1e69b-102">系统 Facet</span><span class="sxs-lookup"><span data-stu-id="1e69b-102">System facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e69b-103">**系统** Facet 指示对象由系统为其自己的操作进行管理。</span><span class="sxs-lookup"><span data-stu-id="1e69b-103">The **System** facet indicates that the object is managed by the system for its own operation.</span></span>
<span data-ttu-id="1e69b-104">大多数应用应忽略具有系统 Facet 的项。</span><span class="sxs-lookup"><span data-stu-id="1e69b-104">Most apps should ignore items that have a System facet.</span></span>

<span data-ttu-id="1e69b-105">**注意**：尽管此 Facet 暂为空，但在今后推出的 API 版本中将在此 Facet 中填充其他属性。</span><span class="sxs-lookup"><span data-stu-id="1e69b-105">**Note**: While this facet is empty today, in future API revisions the facet may be populated with additional properties.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e69b-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e69b-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.systemFacet", "@type.aka": "microsoft.graph.systemFacet" } -->

```json
{
}
```

## <a name="properties"></a><span data-ttu-id="1e69b-107">属性</span><span class="sxs-lookup"><span data-stu-id="1e69b-107">Properties</span></span>

<span data-ttu-id="1e69b-108">无。</span><span class="sxs-lookup"><span data-stu-id="1e69b-108">None.</span></span> <span data-ttu-id="1e69b-109">此 Facet 的值可以为 null，也可以不为 null，但不含任何属性。</span><span class="sxs-lookup"><span data-stu-id="1e69b-109">This facet is a null or not-null value and contains no properties.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/System",
  "suppressions": [
    "Error: /api-reference/beta/resources/systemfacet.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
