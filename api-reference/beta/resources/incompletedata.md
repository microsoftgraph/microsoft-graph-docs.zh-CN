---
author: daspek
description: IncompleteData facet 指示资源是使用不完整的数据生成的。
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 23d78fa3605259031fc2c408e93a0461bb12cb28
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006281"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="17176-103">incompleteData 资源类型</span><span class="sxs-lookup"><span data-stu-id="17176-103">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17176-104">**IncompleteData** facet 指示资源是使用不完整的数据生成的。</span><span class="sxs-lookup"><span data-stu-id="17176-104">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="17176-105">中的属性可能提供了有关不完整数据的原因的信息。</span><span class="sxs-lookup"><span data-stu-id="17176-105">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="17176-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="17176-106">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="17176-107">属性</span><span class="sxs-lookup"><span data-stu-id="17176-107">Properties</span></span>

| <span data-ttu-id="17176-108">属性</span><span class="sxs-lookup"><span data-stu-id="17176-108">Property</span></span>                  | <span data-ttu-id="17176-109">类型</span><span class="sxs-lookup"><span data-stu-id="17176-109">Type</span></span>           | <span data-ttu-id="17176-110">说明</span><span class="sxs-lookup"><span data-stu-id="17176-110">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="17176-111">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="17176-111">missingDataBeforeDateTime</span></span> | <span data-ttu-id="17176-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17176-112">DateTimeOffset</span></span> | <span data-ttu-id="17176-113">该服务在指定的时间之前没有源数据。</span><span class="sxs-lookup"><span data-stu-id="17176-113">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="17176-114">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="17176-114">wasThrottled</span></span>              | <span data-ttu-id="17176-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="17176-115">Boolean</span></span>        | <span data-ttu-id="17176-116">由于活动过多而未记录某些数据。</span><span class="sxs-lookup"><span data-stu-id="17176-116">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
