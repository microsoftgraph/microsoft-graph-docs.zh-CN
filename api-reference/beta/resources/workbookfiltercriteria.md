---
title: workbookFilterCriteria 资源类型
description: 表示应用于列的筛选条件。
localization_priority: Normal
ms.openlocfilehash: 4906a44c88fdd7cb071b4ea994fee609cda1151c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348595"
---
# <a name="workbookfiltercriteria-resource-type"></a><span data-ttu-id="949ca-103">workbookFilterCriteria 资源类型</span><span class="sxs-lookup"><span data-stu-id="949ca-103">workbookFilterCriteria resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="949ca-104">表示应用于列的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="949ca-104">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="949ca-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="949ca-105">JSON representation</span></span>

<span data-ttu-id="949ca-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="949ca-106">Here is a JSON representation of the resource.</span></span>

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
  "values": {"@odata.type":"microsoft.graph.Json"},
  "icon":{"@odata.type": "microsoft.graph.workbookIcon"},
  "operator":"string"
}
```
