---
author: daspek
title: incompleteData 资源类型
description: 不完整Data Facet 指示资源是使用不完整数据生成的。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 20dda8e9d1cd321a465c7a257cb5cb7bed845351
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50239931"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="2114d-103">incompleteData 资源类型</span><span class="sxs-lookup"><span data-stu-id="2114d-103">incompleteData resource type</span></span>

<span data-ttu-id="2114d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2114d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2114d-105">不完整 **Data** Facet 指示资源是使用不完整数据生成的。</span><span class="sxs-lookup"><span data-stu-id="2114d-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="2114d-106">其中的属性可能会提供有关数据不完整的原因的信息。</span><span class="sxs-lookup"><span data-stu-id="2114d-106">The properties within might provide information about why the data is incomplete.</span></span>

## <a name="properties"></a><span data-ttu-id="2114d-107">属性</span><span class="sxs-lookup"><span data-stu-id="2114d-107">Properties</span></span>

| <span data-ttu-id="2114d-108">属性</span><span class="sxs-lookup"><span data-stu-id="2114d-108">Property</span></span>                  | <span data-ttu-id="2114d-109">类型</span><span class="sxs-lookup"><span data-stu-id="2114d-109">Type</span></span>           | <span data-ttu-id="2114d-110">说明</span><span class="sxs-lookup"><span data-stu-id="2114d-110">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="2114d-111">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="2114d-111">missingDataBeforeDateTime</span></span> | <span data-ttu-id="2114d-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2114d-112">DateTimeOffset</span></span> | <span data-ttu-id="2114d-113">服务在指定的时间之前没有源数据。</span><span class="sxs-lookup"><span data-stu-id="2114d-113">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="2114d-114">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="2114d-114">wasThrottled</span></span>              | <span data-ttu-id="2114d-115">布尔</span><span class="sxs-lookup"><span data-stu-id="2114d-115">Boolean</span></span>        | <span data-ttu-id="2114d-116">由于活动过多，某些数据未记录。</span><span class="sxs-lookup"><span data-stu-id="2114d-116">Some data was not recorded due to excessive activity.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2114d-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2114d-117">JSON representation</span></span>

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

