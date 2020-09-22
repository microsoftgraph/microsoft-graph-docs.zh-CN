---
title: printUsageSummaryByUser 资源类型
description: 描述用户在指定时间段内的打印活动 (usageDate) 。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: bba9f57799a36bef4a90b7c514a5be4b4846565e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48070645"
---
# <a name="printusagesummarybyuser-resource-type"></a><span data-ttu-id="cf72a-103">printUsageSummaryByUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf72a-103">printUsageSummaryByUser resource type</span></span>

<span data-ttu-id="cf72a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf72a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf72a-105">描述用户在指定时间段内的打印活动 (usageDate) 。</span><span class="sxs-lookup"><span data-stu-id="cf72a-105">Describes print activity for a user during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="cf72a-106">方法</span><span class="sxs-lookup"><span data-stu-id="cf72a-106">Methods</span></span>

| <span data-ttu-id="cf72a-107">方法</span><span class="sxs-lookup"><span data-stu-id="cf72a-107">Method</span></span>       | <span data-ttu-id="cf72a-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="cf72a-108">Return Type</span></span> | <span data-ttu-id="cf72a-109">说明</span><span class="sxs-lookup"><span data-stu-id="cf72a-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cf72a-110">列出 (每日) </span><span class="sxs-lookup"><span data-stu-id="cf72a-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagesummariesbyuser.md) | [<span data-ttu-id="cf72a-111">printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="cf72a-111">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="cf72a-112">获取按用户分组的每日打印使用率摘要列表。</span><span class="sxs-lookup"><span data-stu-id="cf72a-112">Get a list of daily print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="cf72a-113">每月 () 列表 </span><span class="sxs-lookup"><span data-stu-id="cf72a-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagesummariesbyuser.md) | [<span data-ttu-id="cf72a-114">printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="cf72a-114">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="cf72a-115">获取按月打印的使用情况摘要列表，按用户分组。</span><span class="sxs-lookup"><span data-stu-id="cf72a-115">Get a list of monthly print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="cf72a-116">Get</span><span class="sxs-lookup"><span data-stu-id="cf72a-116">Get</span></span>](../api/printusagesummarybyuser-get.md) | [<span data-ttu-id="cf72a-117">printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="cf72a-117">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="cf72a-118">读取 printUsageSummaryByUser 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cf72a-118">Read properties and relationships of a printUsageSummaryByUser object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cf72a-119">属性</span><span class="sxs-lookup"><span data-stu-id="cf72a-119">Properties</span></span>
| <span data-ttu-id="cf72a-120">属性</span><span class="sxs-lookup"><span data-stu-id="cf72a-120">Property</span></span>     | <span data-ttu-id="cf72a-121">类型</span><span class="sxs-lookup"><span data-stu-id="cf72a-121">Type</span></span>        | <span data-ttu-id="cf72a-122">说明</span><span class="sxs-lookup"><span data-stu-id="cf72a-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cf72a-123">id</span><span class="sxs-lookup"><span data-stu-id="cf72a-123">id</span></span>|<span data-ttu-id="cf72a-124">String</span><span class="sxs-lookup"><span data-stu-id="cf72a-124">String</span></span>|<span data-ttu-id="cf72a-125">此使用率摘要的 ID。</span><span class="sxs-lookup"><span data-stu-id="cf72a-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="cf72a-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cf72a-126">userPrincipalName</span></span>|<span data-ttu-id="cf72a-127">String</span><span class="sxs-lookup"><span data-stu-id="cf72a-127">String</span></span>|<span data-ttu-id="cf72a-128">由这些统计信息表示的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="cf72a-128">The UPN of the user represented by these statistics.</span></span>|
|<span data-ttu-id="cf72a-129">usageDate</span><span class="sxs-lookup"><span data-stu-id="cf72a-129">usageDate</span></span>|<span data-ttu-id="cf72a-130">日期</span><span class="sxs-lookup"><span data-stu-id="cf72a-130">Date</span></span>|<span data-ttu-id="cf72a-131">与这些统计信息关联的日期。</span><span class="sxs-lookup"><span data-stu-id="cf72a-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="cf72a-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="cf72a-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="cf72a-133">Int64</span><span class="sxs-lookup"><span data-stu-id="cf72a-133">Int64</span></span>|<span data-ttu-id="cf72a-134">在关联日期代表用户完成的黑色和白色打印作业的数量。</span><span class="sxs-lookup"><span data-stu-id="cf72a-134">The number of black and white print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="cf72a-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="cf72a-135">completedColorJobCount</span></span>|<span data-ttu-id="cf72a-136">Int64</span><span class="sxs-lookup"><span data-stu-id="cf72a-136">Int64</span></span>|<span data-ttu-id="cf72a-137">在关联日期代表用户完成的彩色打印作业的数量。</span><span class="sxs-lookup"><span data-stu-id="cf72a-137">The number of color print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="cf72a-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="cf72a-138">incompleteJobCount</span></span>|<span data-ttu-id="cf72a-139">Int64</span><span class="sxs-lookup"><span data-stu-id="cf72a-139">Int64</span></span>|<span data-ttu-id="cf72a-140">在关联的日期上代表用户排队但未完成的打印作业数。</span><span class="sxs-lookup"><span data-stu-id="cf72a-140">The number of print jobs that were queued on behalf of the user, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf72a-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf72a-141">JSON representation</span></span>

<span data-ttu-id="cf72a-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf72a-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageSummaryByUser"
}-->

```json
{
    "id": "String (identifier)",
    "userPrincipalName": "String (identifier)",
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
  "description": "printUsageSummaryByUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

