---
author: daspek
ms.author: dspektor
ms.date: 10/06/2017
title: IncompleteData
localization_priority: Normal
ms.openlocfilehash: f2493263d5293b95cbe386b46c56429d11dda089
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549032"
---
# <a name="incompletedata-resource-type"></a><span data-ttu-id="fb8ee-102">incompleteData 资源类型</span><span class="sxs-lookup"><span data-stu-id="fb8ee-102">incompleteData resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb8ee-103">**incompleteData** facet 指示资源是使用不完整的数据生成的。</span><span class="sxs-lookup"><span data-stu-id="fb8ee-103">The **incompleteData** facet indicates that a resource was generated with incomplete data.</span></span>
<span data-ttu-id="fb8ee-104">中的属性可能提供了有关不完整数据的原因的信息。</span><span class="sxs-lookup"><span data-stu-id="fb8ee-104">The properties within may provide information about why there is incomplete data.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fb8ee-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fb8ee-105">JSON representation</span></span>

<!-- { "blockType": "resource", "@type": "microsoft.graph.incompleteData" } -->

```json
{
  "missingDataBeforeDateTime": "String (timestamp)",
  "wasThrottled": false
}
```

## <a name="properties"></a><span data-ttu-id="fb8ee-106">属性</span><span class="sxs-lookup"><span data-stu-id="fb8ee-106">Properties</span></span>

| <span data-ttu-id="fb8ee-107">属性</span><span class="sxs-lookup"><span data-stu-id="fb8ee-107">Property</span></span>                  | <span data-ttu-id="fb8ee-108">类型</span><span class="sxs-lookup"><span data-stu-id="fb8ee-108">Type</span></span>           | <span data-ttu-id="fb8ee-109">说明</span><span class="sxs-lookup"><span data-stu-id="fb8ee-109">Description</span></span>
|:--------------------------|:---------------|:--------------------------------
| <span data-ttu-id="fb8ee-110">missingDataBeforeDateTime</span><span class="sxs-lookup"><span data-stu-id="fb8ee-110">missingDataBeforeDateTime</span></span> | <span data-ttu-id="fb8ee-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fb8ee-111">DateTimeOffset</span></span> | <span data-ttu-id="fb8ee-112">该服务在指定的时间之前没有源数据。</span><span class="sxs-lookup"><span data-stu-id="fb8ee-112">The service does not have source data before the specified time.</span></span>
| <span data-ttu-id="fb8ee-113">wasThrottled</span><span class="sxs-lookup"><span data-stu-id="fb8ee-113">wasThrottled</span></span>              | <span data-ttu-id="fb8ee-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="fb8ee-114">Boolean</span></span>        | <span data-ttu-id="fb8ee-115">由于活动过多而未记录某些数据。</span><span class="sxs-lookup"><span data-stu-id="fb8ee-115">Some data was not recorded due to excessive activity.</span></span>

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
