---
title: FilterCriteria 资源类型
description: 表示应用于列的筛选条件。
localization_priority: Normal
ms.openlocfilehash: 784615f6fce3dea5041772a15e3573c22dabdfd0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522446"
---
# <a name="filtercriteria-resource-type"></a><span data-ttu-id="9395c-103">FilterCriteria 资源类型</span><span class="sxs-lookup"><span data-stu-id="9395c-103">FilterCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9395c-104">表示应用于列的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="9395c-104">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9395c-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9395c-105">JSON representation</span></span>

<span data-ttu-id="9395c-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9395c-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.filterCriteria"
}-->

```json
{
  "color": "string",
  "criterion1": "string",
  "criterion2": "string",
  "dynamicCriteria": "string",
  "filterOn": "string",
  "values": "string"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/filtercriteria.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
