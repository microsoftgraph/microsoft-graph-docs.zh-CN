---
author: daspek
ms.author: dspektor
title: incompleteData 资源类型
description: IncompleteData facet 指示资源是使用不完整的数据生成的。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 0ac77c5dc4daed9330c4fb71185e9505feee5048
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029237"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="d7570-103">incompleteData 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7570-103">incompleteData resource type</span></span>

<span data-ttu-id="d7570-104">**IncompleteData** facet 指示资源是使用不完整的数据生成的。</span><span class="sxs-lookup"><span data-stu-id="d7570-104">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="d7570-105">中的属性可能提供有关数据不完整的原因的信息。</span><span class="sxs-lookup"><span data-stu-id="d7570-105">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="d7570-106">属性</span><span class="sxs-lookup"><span data-stu-id="d7570-106">Properties</span></span>

| <span data-ttu-id="d7570-107">属性</span><span class="sxs-lookup"><span data-stu-id="d7570-107">Property</span></span>                  | <span data-ttu-id="d7570-108">类型</span><span class="sxs-lookup"><span data-stu-id="d7570-108">Type</span></span>           | <span data-ttu-id="d7570-109">说明</span><span class="sxs-lookup"><span data-stu-id="d7570-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="d7570-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="d7570-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="d7570-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d7570-111">DateTimeOffset</span></span> | <span data-ttu-id="d7570-112">该服务在指定的时间之前没有源数据。</span><span class="sxs-lookup"><span data-stu-id="d7570-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="d7570-113">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="d7570-113">wasThrottled</span></span>              | <span data-ttu-id="d7570-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7570-114">Boolean</span></span>        | <span data-ttu-id="d7570-115">由于活动过多而未记录某些数据。</span><span class="sxs-lookup"><span data-stu-id="d7570-115">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7570-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7570-116">JSON representation</span></span>

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
