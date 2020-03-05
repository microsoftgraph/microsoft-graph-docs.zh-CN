---
author: daspek
description: IncompleteData facet 指示资源是使用不完整的数据生成的。
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 3abefff4749413648a3f1a56d1dbf6d44f16a471
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496276"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="ff58a-103">incompleteData 资源类型</span><span class="sxs-lookup"><span data-stu-id="ff58a-103">incompleteData resource type</span></span>

<span data-ttu-id="ff58a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ff58a-104">Namespace: microsoft.graph</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff58a-105">**IncompleteData** facet 指示资源是使用不完整的数据生成的。</span><span class="sxs-lookup"><span data-stu-id="ff58a-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="ff58a-106">中的属性可能提供了有关不完整数据的原因的信息。</span><span class="sxs-lookup"><span data-stu-id="ff58a-106">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff58a-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ff58a-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="ff58a-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff58a-108">Properties</span></span>

| <span data-ttu-id="ff58a-109">属性</span><span class="sxs-lookup"><span data-stu-id="ff58a-109">Property</span></span>                  | <span data-ttu-id="ff58a-110">类型</span><span class="sxs-lookup"><span data-stu-id="ff58a-110">Type</span></span>           | <span data-ttu-id="ff58a-111">说明</span><span class="sxs-lookup"><span data-stu-id="ff58a-111">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="ff58a-112">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="ff58a-112">missingDataBeforeDateTime</span></span> | <span data-ttu-id="ff58a-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff58a-113">DateTimeOffset</span></span> | <span data-ttu-id="ff58a-114">该服务在指定的时间之前没有源数据。</span><span class="sxs-lookup"><span data-stu-id="ff58a-114">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="ff58a-115">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="ff58a-115">wasThrottled</span></span>              | <span data-ttu-id="ff58a-116">布尔</span><span class="sxs-lookup"><span data-stu-id="ff58a-116">Boolean</span></span>        | <span data-ttu-id="ff58a-117">由于活动过多而未记录某些数据。</span><span class="sxs-lookup"><span data-stu-id="ff58a-117">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": []
}
-->
