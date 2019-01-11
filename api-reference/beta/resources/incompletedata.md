---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: add1e3612f65e203f2437419cbb105b78025aa0a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27807509"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="495de-102">incompleteData 资源类型</span><span class="sxs-lookup"><span data-stu-id="495de-102">incompleteData resource type</span></span>

 > <span data-ttu-id="495de-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="495de-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="495de-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="495de-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="495de-105">**IncompleteData**方面指示资源生成不完整的数据。</span><span class="sxs-lookup"><span data-stu-id="495de-105">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="495de-106">内的属性可能提供有关信息，为什么不完整数据。</span><span class="sxs-lookup"><span data-stu-id="495de-106">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="495de-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="495de-107">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="495de-108">属性</span><span class="sxs-lookup"><span data-stu-id="495de-108">Properties</span></span>

| <span data-ttu-id="495de-109">属性</span><span class="sxs-lookup"><span data-stu-id="495de-109">Property</span></span>                  | <span data-ttu-id="495de-110">类型</span><span class="sxs-lookup"><span data-stu-id="495de-110">Type</span></span>           | <span data-ttu-id="495de-111">Description</span><span class="sxs-lookup"><span data-stu-id="495de-111">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="495de-112">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="495de-112">missingDataBeforeDateTime</span></span> | <span data-ttu-id="495de-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="495de-113">DateTimeOffset</span></span> | <span data-ttu-id="495de-114">该服务不具有之前指定的时间的源数据。</span><span class="sxs-lookup"><span data-stu-id="495de-114">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="495de-115">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="495de-115">wasThrottled</span></span>              | <span data-ttu-id="495de-116">布尔</span><span class="sxs-lookup"><span data-stu-id="495de-116">Boolean</span></span>        | <span data-ttu-id="495de-117">由于活动太多而未录制一些数据。</span><span class="sxs-lookup"><span data-stu-id="495de-117">Some data was not recorded due to excessive activity.</span></span>

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData"
} -->
