---
author: daspek
description: IncompleteData facet 指示资源是使用不完整的数据生成的。
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6505d02ee7436e02d90627cfd38a83e3e436706a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016557"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="8bf06-103">incompleteData 资源类型</span><span class="sxs-lookup"><span data-stu-id="8bf06-103">incompleteData resource type</span></span>

<span data-ttu-id="8bf06-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8bf06-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bf06-105">**IncompleteData** facet 指示资源是使用不完整的数据生成的。</span><span class="sxs-lookup"><span data-stu-id="8bf06-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="8bf06-106">中的属性可能提供了有关不完整数据的原因的信息。</span><span class="sxs-lookup"><span data-stu-id="8bf06-106">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8bf06-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8bf06-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="8bf06-108">属性</span><span class="sxs-lookup"><span data-stu-id="8bf06-108">Properties</span></span>

| <span data-ttu-id="8bf06-109">属性</span><span class="sxs-lookup"><span data-stu-id="8bf06-109">Property</span></span>                  | <span data-ttu-id="8bf06-110">类型</span><span class="sxs-lookup"><span data-stu-id="8bf06-110">Type</span></span>           | <span data-ttu-id="8bf06-111">说明</span><span class="sxs-lookup"><span data-stu-id="8bf06-111">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="8bf06-112">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="8bf06-112">missingDataBeforeDateTime</span></span> | <span data-ttu-id="8bf06-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8bf06-113">DateTimeOffset</span></span> | <span data-ttu-id="8bf06-114">该服务在指定的时间之前没有源数据。</span><span class="sxs-lookup"><span data-stu-id="8bf06-114">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="8bf06-115">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="8bf06-115">wasThrottled</span></span>              | <span data-ttu-id="8bf06-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="8bf06-116">Boolean</span></span>        | <span data-ttu-id="8bf06-117">由于活动过多而未记录某些数据。</span><span class="sxs-lookup"><span data-stu-id="8bf06-117">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->


