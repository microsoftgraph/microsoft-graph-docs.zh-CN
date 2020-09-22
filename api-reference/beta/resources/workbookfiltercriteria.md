---
title: workbookFilterCriteria 资源类型
description: 表示应用于列的筛选条件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: 6ad0095b48f39937ab4e8d7d02f533bd9a140ff9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079653"
---
# <a name="workbookfiltercriteria-resource-type"></a><span data-ttu-id="d3b85-103">workbookFilterCriteria 资源类型</span><span class="sxs-lookup"><span data-stu-id="d3b85-103">workbookFilterCriteria resource type</span></span>

<span data-ttu-id="d3b85-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d3b85-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d3b85-105">表示应用于列的筛选条件。</span><span class="sxs-lookup"><span data-stu-id="d3b85-105">Represents the filtering criteria applied to a column.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d3b85-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d3b85-106">JSON representation</span></span>

<span data-ttu-id="d3b85-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d3b85-107">Here is a JSON representation of the resource.</span></span>

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


