---
title: printUsageSummaryByPrinter 资源类型
description: 描述在指定时间段 (usageDate) 时打印机的打印活动。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 4d33ab99780f980dcc24e267ba1ac6603f602aa2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070646"
---
# <a name="printusagesummarybyprinter-resource-type"></a><span data-ttu-id="f40bf-103">printUsageSummaryByPrinter 资源类型</span><span class="sxs-lookup"><span data-stu-id="f40bf-103">printUsageSummaryByPrinter resource type</span></span>

<span data-ttu-id="f40bf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f40bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f40bf-105">描述在指定时间段 (usageDate) 时打印机的打印活动。</span><span class="sxs-lookup"><span data-stu-id="f40bf-105">Describes print activity for a printer during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="f40bf-106">方法</span><span class="sxs-lookup"><span data-stu-id="f40bf-106">Methods</span></span>

| <span data-ttu-id="f40bf-107">方法</span><span class="sxs-lookup"><span data-stu-id="f40bf-107">Method</span></span>       | <span data-ttu-id="f40bf-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f40bf-108">Return Type</span></span> | <span data-ttu-id="f40bf-109">说明</span><span class="sxs-lookup"><span data-stu-id="f40bf-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f40bf-110">列出 (每日) </span><span class="sxs-lookup"><span data-stu-id="f40bf-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagesummariesbyprinter.md) | [<span data-ttu-id="f40bf-111">printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="f40bf-111">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="f40bf-112">获取按打印机分组的每日打印使用率摘要列表。</span><span class="sxs-lookup"><span data-stu-id="f40bf-112">Get a list of daily print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="f40bf-113">每月 () 列表 </span><span class="sxs-lookup"><span data-stu-id="f40bf-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagesummariesbyprinter.md) | [<span data-ttu-id="f40bf-114">printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="f40bf-114">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="f40bf-115">获取按打印机分组的按月打印使用情况摘要列表。</span><span class="sxs-lookup"><span data-stu-id="f40bf-115">Get a list of monthly print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="f40bf-116">Get</span><span class="sxs-lookup"><span data-stu-id="f40bf-116">Get</span></span>](../api/printusagesummarybyprinter-get.md) | [<span data-ttu-id="f40bf-117">printUsageSummaryByPrinter</span><span class="sxs-lookup"><span data-stu-id="f40bf-117">printUsageSummaryByPrinter</span></span>](printusagesummarybyprinter.md) | <span data-ttu-id="f40bf-118">读取 **printUsageSummaryByPrinter** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f40bf-118">Read the properties and relationships of a **printUsageSummaryByPrinter** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f40bf-119">属性</span><span class="sxs-lookup"><span data-stu-id="f40bf-119">Properties</span></span>
| <span data-ttu-id="f40bf-120">属性</span><span class="sxs-lookup"><span data-stu-id="f40bf-120">Property</span></span>     | <span data-ttu-id="f40bf-121">类型</span><span class="sxs-lookup"><span data-stu-id="f40bf-121">Type</span></span>        | <span data-ttu-id="f40bf-122">说明</span><span class="sxs-lookup"><span data-stu-id="f40bf-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f40bf-123">id</span><span class="sxs-lookup"><span data-stu-id="f40bf-123">id</span></span>|<span data-ttu-id="f40bf-124">String</span><span class="sxs-lookup"><span data-stu-id="f40bf-124">String</span></span>|<span data-ttu-id="f40bf-125">此使用率摘要的 ID。</span><span class="sxs-lookup"><span data-stu-id="f40bf-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="f40bf-126">printerID</span><span class="sxs-lookup"><span data-stu-id="f40bf-126">printerID</span></span>|<span data-ttu-id="f40bf-127">String</span><span class="sxs-lookup"><span data-stu-id="f40bf-127">String</span></span>|<span data-ttu-id="f40bf-128">由这些统计信息表示的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="f40bf-128">The ID of the printer represented by these statistics.</span></span>|
|<span data-ttu-id="f40bf-129">usageDate</span><span class="sxs-lookup"><span data-stu-id="f40bf-129">usageDate</span></span>|<span data-ttu-id="f40bf-130">日期</span><span class="sxs-lookup"><span data-stu-id="f40bf-130">Date</span></span>|<span data-ttu-id="f40bf-131">与这些统计信息关联的日期。</span><span class="sxs-lookup"><span data-stu-id="f40bf-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="f40bf-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="f40bf-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="f40bf-133">Int64</span><span class="sxs-lookup"><span data-stu-id="f40bf-133">Int64</span></span>|<span data-ttu-id="f40bf-134">打印机在关联日期完成的黑色和白色打印作业的数量。</span><span class="sxs-lookup"><span data-stu-id="f40bf-134">The number of black and white print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="f40bf-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="f40bf-135">completedColorJobCount</span></span>|<span data-ttu-id="f40bf-136">Int64</span><span class="sxs-lookup"><span data-stu-id="f40bf-136">Int64</span></span>|<span data-ttu-id="f40bf-137">打印机在关联日期完成的彩色打印作业数。</span><span class="sxs-lookup"><span data-stu-id="f40bf-137">The number of color print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="f40bf-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="f40bf-138">incompleteJobCount</span></span>|<span data-ttu-id="f40bf-139">Int64</span><span class="sxs-lookup"><span data-stu-id="f40bf-139">Int64</span></span>|<span data-ttu-id="f40bf-140">在关联的日期上排队等候打印机但尚未完成的打印作业的数量。</span><span class="sxs-lookup"><span data-stu-id="f40bf-140">The number of print jobs that were queued for the printer, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f40bf-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f40bf-141">JSON representation</span></span>

<span data-ttu-id="f40bf-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f40bf-142">The following is a JSON representation of the resource.</span></span>

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

