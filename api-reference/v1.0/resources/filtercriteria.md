---
title: FilterCriteria 资源类型
description: 表示应用于列的筛选条件。
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 38553e51abf8be80740e7eaeded1eb7b17705173
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018296"
---
# <a name="filtercriteria-resource-type"></a><span data-ttu-id="e40e8-103">FilterCriteria 资源类型</span><span class="sxs-lookup"><span data-stu-id="e40e8-103">FilterCriteria resource type</span></span>

<span data-ttu-id="e40e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e40e8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e40e8-105">表示应用于列的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="e40e8-105">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e40e8-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e40e8-106">JSON representation</span></span>

<span data-ttu-id="e40e8-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e40e8-107">Here is a JSON representation of the resource.</span></span>

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

