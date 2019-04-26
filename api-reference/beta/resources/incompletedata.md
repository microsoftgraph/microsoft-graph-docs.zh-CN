---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: 40c1b782384076eefc986f67dc1736f191feb7b7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339963"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="467d9-102">incompleteData 资源类型</span><span class="sxs-lookup"><span data-stu-id="467d9-102">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="467d9-103">**incompleteData** facet 指示资源是使用不完整的数据生成的。</span><span class="sxs-lookup"><span data-stu-id="467d9-103">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="467d9-104">中的属性可能提供了有关不完整数据的原因的信息。</span><span class="sxs-lookup"><span data-stu-id="467d9-104">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="467d9-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="467d9-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="467d9-106">属性</span><span class="sxs-lookup"><span data-stu-id="467d9-106">Properties</span></span>

| <span data-ttu-id="467d9-107">属性</span><span class="sxs-lookup"><span data-stu-id="467d9-107">Property</span></span>                  | <span data-ttu-id="467d9-108">类型</span><span class="sxs-lookup"><span data-stu-id="467d9-108">Type</span></span>           | <span data-ttu-id="467d9-109">说明</span><span class="sxs-lookup"><span data-stu-id="467d9-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="467d9-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="467d9-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="467d9-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="467d9-111">DateTimeOffset</span></span> | <span data-ttu-id="467d9-112">该服务在指定的时间之前没有源数据。</span><span class="sxs-lookup"><span data-stu-id="467d9-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="467d9-113">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="467d9-113">wasThrottled</span></span>              | <span data-ttu-id="467d9-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="467d9-114">Boolean</span></span>        | <span data-ttu-id="467d9-115">由于活动过多而未记录某些数据。</span><span class="sxs-lookup"><span data-stu-id="467d9-115">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
