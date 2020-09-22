---
author: daspek
ms.author: dspektor
title: incompleteData 资源类型
description: IncompleteData facet 指示资源是使用不完整的数据生成的。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 424a857468473532dc6f2a39c4c13dc94b52406c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48054887"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="ee305-103">incompleteData 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee305-103">incompleteData resource type</span></span>

<span data-ttu-id="ee305-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ee305-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ee305-105">**IncompleteData** facet 指示资源是使用不完整的数据生成的。</span><span class="sxs-lookup"><span data-stu-id="ee305-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="ee305-106">中的属性可能提供有关数据不完整的原因的信息。</span><span class="sxs-lookup"><span data-stu-id="ee305-106">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="ee305-107">属性</span><span class="sxs-lookup"><span data-stu-id="ee305-107">Properties</span></span>

| <span data-ttu-id="ee305-108">属性</span><span class="sxs-lookup"><span data-stu-id="ee305-108">Property</span></span>                  | <span data-ttu-id="ee305-109">类型</span><span class="sxs-lookup"><span data-stu-id="ee305-109">Type</span></span>           | <span data-ttu-id="ee305-110">说明</span><span class="sxs-lookup"><span data-stu-id="ee305-110">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="ee305-111">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="ee305-111">missingDataBeforeDateTime</span></span> | <span data-ttu-id="ee305-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee305-112">DateTimeOffset</span></span> | <span data-ttu-id="ee305-113">该服务在指定的时间之前没有源数据。</span><span class="sxs-lookup"><span data-stu-id="ee305-113">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="ee305-114">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="ee305-114">wasThrottled</span></span>              | <span data-ttu-id="ee305-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee305-115">Boolean</span></span>        | <span data-ttu-id="ee305-116">由于活动过多而未记录某些数据。</span><span class="sxs-lookup"><span data-stu-id="ee305-116">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee305-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee305-117">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/incompleteData",
  "suppressions": []
}
-->

