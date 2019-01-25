---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: f2493263d5293b95cbe386b46c56429d11dda089
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29525085"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="0f95f-102">incompleteData 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f95f-102">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0f95f-103">**IncompleteData**方面指示资源生成不完整的数据。</span><span class="sxs-lookup"><span data-stu-id="0f95f-103">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="0f95f-104">内的属性可能提供有关信息，为什么不完整数据。</span><span class="sxs-lookup"><span data-stu-id="0f95f-104">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f95f-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f95f-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="0f95f-106">属性</span><span class="sxs-lookup"><span data-stu-id="0f95f-106">Properties</span></span>

| <span data-ttu-id="0f95f-107">属性</span><span class="sxs-lookup"><span data-stu-id="0f95f-107">Property</span></span>                  | <span data-ttu-id="0f95f-108">类型</span><span class="sxs-lookup"><span data-stu-id="0f95f-108">Type</span></span>           | <span data-ttu-id="0f95f-109">说明</span><span class="sxs-lookup"><span data-stu-id="0f95f-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="0f95f-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="0f95f-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="0f95f-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f95f-111">DateTimeOffset</span></span> | <span data-ttu-id="0f95f-112">该服务不具有之前指定的时间的源数据。</span><span class="sxs-lookup"><span data-stu-id="0f95f-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="0f95f-113">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="0f95f-113">wasThrottled</span></span>              | <span data-ttu-id="0f95f-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f95f-114">Boolean</span></span>        | <span data-ttu-id="0f95f-115">由于活动太多而未录制一些数据。</span><span class="sxs-lookup"><span data-stu-id="0f95f-115">Some data was not recorded due to excessive activity.</span></span>

<!--
{
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Facets/IncompleteData",
  "suppressions": [
    "Error: /api-reference/beta/resources/incompletedata.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
