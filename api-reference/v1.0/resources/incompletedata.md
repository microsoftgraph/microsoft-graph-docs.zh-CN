---
author: daspek
ms.author: dspektor
title: incompleteData 资源类型
description: IncompleteData facet 指示资源是使用不完整的数据生成的。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f26317cf16f0773852df35941c00e88df145cc31
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970655"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="780f6-103">incompleteData 资源类型</span><span class="sxs-lookup"><span data-stu-id="780f6-103">incompleteData resource type</span></span>

<span data-ttu-id="780f6-104">**IncompleteData** facet 指示资源是使用不完整的数据生成的。</span><span class="sxs-lookup"><span data-stu-id="780f6-104">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="780f6-105">中的属性可能提供有关数据不完整的原因的信息。</span><span class="sxs-lookup"><span data-stu-id="780f6-105">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="780f6-106">属性</span><span class="sxs-lookup"><span data-stu-id="780f6-106">Properties</span></span>

| <span data-ttu-id="780f6-107">属性</span><span class="sxs-lookup"><span data-stu-id="780f6-107">Property</span></span>                  | <span data-ttu-id="780f6-108">类型</span><span class="sxs-lookup"><span data-stu-id="780f6-108">Type</span></span>           | <span data-ttu-id="780f6-109">说明</span><span class="sxs-lookup"><span data-stu-id="780f6-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="780f6-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="780f6-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="780f6-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="780f6-111">DateTimeOffset</span></span> | <span data-ttu-id="780f6-112">该服务在指定的时间之前没有源数据。</span><span class="sxs-lookup"><span data-stu-id="780f6-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="780f6-113">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="780f6-113">wasThrottled</span></span>              | <span data-ttu-id="780f6-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="780f6-114">Boolean</span></span>        | <span data-ttu-id="780f6-115">由于活动过多而未记录某些数据。</span><span class="sxs-lookup"><span data-stu-id="780f6-115">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="780f6-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="780f6-116">JSON representation</span></span>

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
