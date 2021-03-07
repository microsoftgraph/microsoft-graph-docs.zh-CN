---
title: printUsageByPrinter 资源类型
description: 描述指定时间段内打印机的打印活动 (usageDate) 。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 8c5a69d01f0b8da05a5f72f5c2c7d9bacf10ff1a
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517261"
---
# <a name="printusagebyprinter-resource-type"></a><span data-ttu-id="1d23e-103">printUsageByPrinter 资源类型</span><span class="sxs-lookup"><span data-stu-id="1d23e-103">printUsageByPrinter resource type</span></span>

<span data-ttu-id="1d23e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d23e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="1d23e-105">描述指定时间段内打印机的打印活动 (usageDate) 。</span><span class="sxs-lookup"><span data-stu-id="1d23e-105">Describes print activity for a printer during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="1d23e-106">Methods</span><span class="sxs-lookup"><span data-stu-id="1d23e-106">Methods</span></span>
|<span data-ttu-id="1d23e-107">方法</span><span class="sxs-lookup"><span data-stu-id="1d23e-107">Method</span></span>|<span data-ttu-id="1d23e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1d23e-108">Return type</span></span>|<span data-ttu-id="1d23e-109">Description</span><span class="sxs-lookup"><span data-stu-id="1d23e-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="1d23e-110">列出 (每天) </span><span class="sxs-lookup"><span data-stu-id="1d23e-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagebyprinter.md) | [<span data-ttu-id="1d23e-111">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="1d23e-111">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="1d23e-112">获取按打印机分组的每日打印使用率摘要的列表。</span><span class="sxs-lookup"><span data-stu-id="1d23e-112">Get a list of daily print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="1d23e-113">列出 (每月) </span><span class="sxs-lookup"><span data-stu-id="1d23e-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagebyprinter.md) | [<span data-ttu-id="1d23e-114">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="1d23e-114">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="1d23e-115">获取按打印机分组的每月打印使用率摘要的列表。</span><span class="sxs-lookup"><span data-stu-id="1d23e-115">Get a list of monthly print usage summaries, grouped by printer.</span></span> |
| [<span data-ttu-id="1d23e-116">获取</span><span class="sxs-lookup"><span data-stu-id="1d23e-116">Get</span></span>](../api/printUsageByPrinter-get.md) | [<span data-ttu-id="1d23e-117">printUsageByPrinter</span><span class="sxs-lookup"><span data-stu-id="1d23e-117">printUsageByPrinter</span></span>](printUsageByPrinter.md) | <span data-ttu-id="1d23e-118">读取 **printUsageByPrinter** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1d23e-118">Read the properties and relationships of a **printUsageByPrinter** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1d23e-119">属性</span><span class="sxs-lookup"><span data-stu-id="1d23e-119">Properties</span></span>
|<span data-ttu-id="1d23e-120">属性</span><span class="sxs-lookup"><span data-stu-id="1d23e-120">Property</span></span>|<span data-ttu-id="1d23e-121">类型</span><span class="sxs-lookup"><span data-stu-id="1d23e-121">Type</span></span>|<span data-ttu-id="1d23e-122">说明</span><span class="sxs-lookup"><span data-stu-id="1d23e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d23e-123">id</span><span class="sxs-lookup"><span data-stu-id="1d23e-123">id</span></span>|<span data-ttu-id="1d23e-124">String</span><span class="sxs-lookup"><span data-stu-id="1d23e-124">String</span></span>|<span data-ttu-id="1d23e-125">此使用率摘要的 ID。</span><span class="sxs-lookup"><span data-stu-id="1d23e-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="1d23e-126">printerID</span><span class="sxs-lookup"><span data-stu-id="1d23e-126">printerID</span></span>|<span data-ttu-id="1d23e-127">String</span><span class="sxs-lookup"><span data-stu-id="1d23e-127">String</span></span>|<span data-ttu-id="1d23e-128">由这些统计信息表示的打印机的 ID。</span><span class="sxs-lookup"><span data-stu-id="1d23e-128">The ID of the printer represented by these statistics.</span></span>|
|<span data-ttu-id="1d23e-129">usageDate</span><span class="sxs-lookup"><span data-stu-id="1d23e-129">usageDate</span></span>|<span data-ttu-id="1d23e-130">日期</span><span class="sxs-lookup"><span data-stu-id="1d23e-130">Date</span></span>|<span data-ttu-id="1d23e-131">与这些统计信息关联的日期。</span><span class="sxs-lookup"><span data-stu-id="1d23e-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="1d23e-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="1d23e-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="1d23e-133">Int64</span><span class="sxs-lookup"><span data-stu-id="1d23e-133">Int64</span></span>|<span data-ttu-id="1d23e-134">打印机在关联日期完成的黑白打印作业数。</span><span class="sxs-lookup"><span data-stu-id="1d23e-134">The number of black and white print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="1d23e-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="1d23e-135">completedColorJobCount</span></span>|<span data-ttu-id="1d23e-136">Int64</span><span class="sxs-lookup"><span data-stu-id="1d23e-136">Int64</span></span>|<span data-ttu-id="1d23e-137">打印机在关联日期完成的颜色打印作业数。</span><span class="sxs-lookup"><span data-stu-id="1d23e-137">The number of color print jobs completed by the printer on the associated date.</span></span>|
|<span data-ttu-id="1d23e-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="1d23e-138">incompleteJobCount</span></span>|<span data-ttu-id="1d23e-139">Int64</span><span class="sxs-lookup"><span data-stu-id="1d23e-139">Int64</span></span>|<span data-ttu-id="1d23e-140">在关联日期排入打印机队列但未完成的打印作业数。</span><span class="sxs-lookup"><span data-stu-id="1d23e-140">The number of print jobs that were queued for the printer, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1d23e-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1d23e-141">JSON representation</span></span>
<span data-ttu-id="1d23e-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1d23e-142">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printUsageByPrinter",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printUsageByPrinter",
  "id": "String (identifier)",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "printerId": "String"
}
```

