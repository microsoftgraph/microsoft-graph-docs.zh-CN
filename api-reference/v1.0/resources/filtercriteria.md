---
title: FilterCriteria 资源类型
description: 表示应用于列的筛选条件。
ms.openlocfilehash: 7fafbf8ef71eac9cf4896927f38ed1add5da9320
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011419"
---
# <a name="filtercriteria-resource-type"></a><span data-ttu-id="3f64d-103">FilterCriteria 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f64d-103">FilterCriteria resource type</span></span>

<span data-ttu-id="3f64d-104">表示应用于列的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="3f64d-104">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f64d-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f64d-105">JSON representation</span></span>

<span data-ttu-id="3f64d-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f64d-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "icon": {"@odata.type": "microsoft.graph.workbookIcon"},
  "values": {"@odata.type": "microsoft.graph.Json"}
}

```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'color' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'criterion1' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'criterion2' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'dynamicCriteria' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'filterOn' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'icon' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table.",
    "Warning: /api-reference/v1.0/resources/filtercriteria.md:
      Property 'values' found in resource definition for 'microsoft.graph.workbookFilterCriteria', but not described in markdown table."
  ]
} -->