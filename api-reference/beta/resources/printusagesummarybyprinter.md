---
title: printUsageSummaryByPrinter 资源类型
description: 描述在指定时间段（usageDate）的打印机的打印活动。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 86d7b4eb107ac6e2732e32bf55a65a7125edb529
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895620"
---
# <a name="printusagesummarybyprinter-resource-type"></a><span data-ttu-id="d0957-103">printUsageSummaryByPrinter 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0957-103">printUsageSummaryByPrinter resource type</span></span>

<span data-ttu-id="d0957-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d0957-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0957-105">描述在指定时间段（usageDate）的打印机的打印活动。</span><span class="sxs-lookup"><span data-stu-id="d0957-105">Describes print activity for a printer during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="d0957-106">方法</span><span class="sxs-lookup"><span data-stu-id="d0957-106">Methods</span></span>

| <span data-ttu-id="d0957-107">方法</span><span class="sxs-lookup"><span data-stu-id="d0957-107">Method</span></span>       | <span data-ttu-id="d0957-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d0957-108">Return Type</span></span> | <span data-ttu-id="d0957-109">说明</span><span class="sxs-lookup"><span data-stu-id="d0957-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="d0957-110">列表（每天）</span><span class="sxs-lookup"><span data-stu-id="d0957-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagesummariesbyprinter.md) | [<span data-ttu-id="d0957-111">printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="d0957-111">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="d0957-112">获取按打印机分组的每日打印使用率摘要列表。</span><span class="sxs-lookup"><span data-stu-id="d0957-112">Get a list of daily print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="d0957-113">列表（每月）</span><span class="sxs-lookup"><span data-stu-id="d0957-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagesummariesbyprinter.md) | [<span data-ttu-id="d0957-114">printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="d0957-114">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="d0957-115">获取按打印机分组的按月打印使用情况摘要列表。</span><span class="sxs-lookup"><span data-stu-id="d0957-115">Get a list of monthly print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="d0957-116">Get</span><span class="sxs-lookup"><span data-stu-id="d0957-116">Get</span></span>](../api/printusagesummarybyprinter-get.md) | [<span data-ttu-id="d0957-117">printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="d0957-117">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="d0957-118">读取**printUsageSummaryByPrinter**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d0957-118">Read the properties and relationships of a **printUsageSummaryByPrinter** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="d0957-119">属性</span><span class="sxs-lookup"><span data-stu-id="d0957-119">Properties</span></span>
| <span data-ttu-id="d0957-120">属性</span><span class="sxs-lookup"><span data-stu-id="d0957-120">Property</span></span>     | <span data-ttu-id="d0957-121">类型</span><span class="sxs-lookup"><span data-stu-id="d0957-121">Type</span></span>        | <span data-ttu-id="d0957-122">说明</span><span class="sxs-lookup"><span data-stu-id="d0957-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d0957-123">id</span><span class="sxs-lookup"><span data-stu-id="d0957-123">id</span></span>|<span data-ttu-id="d0957-124">String</span><span class="sxs-lookup"><span data-stu-id="d0957-124">String</span></span>|<span data-ttu-id="d0957-125">此使用率摘要的 ID。</span><span class="sxs-lookup"><span data-stu-id="d0957-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="d0957-126">printerID</span><span class="sxs-lookup"><span data-stu-id="d0957-126">printerID</span></span>|<span data-ttu-id="d0957-127">String</span><span class="sxs-lookup"><span data-stu-id="d0957-127">String</span></span>|<span data-ttu-id="d0957-128">由这些统计信息表示的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="d0957-128">The ID of the printer represented by these statistics.</span></span>|
|<span data-ttu-id="d0957-129">usageDate</span><span class="sxs-lookup"><span data-stu-id="d0957-129">usageDate</span></span>|<span data-ttu-id="d0957-130">日期</span><span class="sxs-lookup"><span data-stu-id="d0957-130">Date</span></span>|<span data-ttu-id="d0957-131">与这些统计信息关联的日期。</span><span class="sxs-lookup"><span data-stu-id="d0957-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="d0957-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="d0957-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="d0957-133">Int64</span><span class="sxs-lookup"><span data-stu-id="d0957-133">Int64</span></span>|<span data-ttu-id="d0957-134">打印机在关联日期完成的黑色和白色打印作业的数量。</span><span class="sxs-lookup"><span data-stu-id="d0957-134">The number of black and white print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="d0957-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="d0957-135">completedColorJobCount</span></span>|<span data-ttu-id="d0957-136">Int64</span><span class="sxs-lookup"><span data-stu-id="d0957-136">Int64</span></span>|<span data-ttu-id="d0957-137">打印机在关联日期完成的彩色打印作业数。</span><span class="sxs-lookup"><span data-stu-id="d0957-137">The number of color print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="d0957-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="d0957-138">incompleteJobCount</span></span>|<span data-ttu-id="d0957-139">Int64</span><span class="sxs-lookup"><span data-stu-id="d0957-139">Int64</span></span>|<span data-ttu-id="d0957-140">在关联的日期上排队等候打印机但尚未完成的打印作业的数量。</span><span class="sxs-lookup"><span data-stu-id="d0957-140">The number of print jobs that were queued for the printer, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d0957-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0957-141">JSON representation</span></span>

<span data-ttu-id="d0957-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0957-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageSummaryByPrinter"
}-->

```json
{
    "id": "String (identifier)",
    "printerId": "String (identifier)",
    "usageDate": "String (timestamp)",
    "completedBlackAndWhiteJobCount": 123456,
    "completedColorJobCount": 123456,
    "incompleteJobCount": 123456
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printUsageSummaryByPrinter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->