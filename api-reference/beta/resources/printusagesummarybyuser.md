---
title: printUsageSummaryByUser 资源类型
description: 描述在指定时间段（usageDate）期间用户的打印活动。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 30769d9bd7ee76494b1582a3d7afc8a7f75bb07a
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895597"
---
# <a name="printusagesummarybyuser-resource-type"></a><span data-ttu-id="b9a8e-103">printUsageSummaryByUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9a8e-103">printUsageSummaryByUser resource type</span></span>

<span data-ttu-id="b9a8e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9a8e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9a8e-105">描述在指定时间段（usageDate）期间用户的打印活动。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-105">Describes print activity for a user during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="b9a8e-106">方法</span><span class="sxs-lookup"><span data-stu-id="b9a8e-106">Methods</span></span>

| <span data-ttu-id="b9a8e-107">方法</span><span class="sxs-lookup"><span data-stu-id="b9a8e-107">Method</span></span>       | <span data-ttu-id="b9a8e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b9a8e-108">Return Type</span></span> | <span data-ttu-id="b9a8e-109">说明</span><span class="sxs-lookup"><span data-stu-id="b9a8e-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="b9a8e-110">列表（每天）</span><span class="sxs-lookup"><span data-stu-id="b9a8e-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagesummariesbyuser.md) | [<span data-ttu-id="b9a8e-111">printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="b9a8e-111">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="b9a8e-112">获取按用户分组的每日打印使用率摘要列表。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-112">Get a list of daily print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="b9a8e-113">列表（每月）</span><span class="sxs-lookup"><span data-stu-id="b9a8e-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagesummariesbyuser.md) | [<span data-ttu-id="b9a8e-114">printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="b9a8e-114">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="b9a8e-115">获取按月打印的使用情况摘要列表，按用户分组。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-115">Get a list of monthly print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="b9a8e-116">Get</span><span class="sxs-lookup"><span data-stu-id="b9a8e-116">Get</span></span>](../api/printusagesummarybyuser-get.md) | [<span data-ttu-id="b9a8e-117">printUsageSummaryByUser</span><span class="sxs-lookup"><span data-stu-id="b9a8e-117">printUsageSummaryByUser</span></span>](printusagesummarybyuser.md) | <span data-ttu-id="b9a8e-118">读取 printUsageSummaryByUser 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-118">Read properties and relationships of a printUsageSummaryByUser object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b9a8e-119">属性</span><span class="sxs-lookup"><span data-stu-id="b9a8e-119">Properties</span></span>
| <span data-ttu-id="b9a8e-120">属性</span><span class="sxs-lookup"><span data-stu-id="b9a8e-120">Property</span></span>     | <span data-ttu-id="b9a8e-121">类型</span><span class="sxs-lookup"><span data-stu-id="b9a8e-121">Type</span></span>        | <span data-ttu-id="b9a8e-122">说明</span><span class="sxs-lookup"><span data-stu-id="b9a8e-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9a8e-123">id</span><span class="sxs-lookup"><span data-stu-id="b9a8e-123">id</span></span>|<span data-ttu-id="b9a8e-124">String</span><span class="sxs-lookup"><span data-stu-id="b9a8e-124">String</span></span>|<span data-ttu-id="b9a8e-125">此使用率摘要的 ID。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="b9a8e-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b9a8e-126">userPrincipalName</span></span>|<span data-ttu-id="b9a8e-127">String</span><span class="sxs-lookup"><span data-stu-id="b9a8e-127">String</span></span>|<span data-ttu-id="b9a8e-128">由这些统计信息表示的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-128">The UPN of the user represented by these statistics.</span></span>|
|<span data-ttu-id="b9a8e-129">usageDate</span><span class="sxs-lookup"><span data-stu-id="b9a8e-129">usageDate</span></span>|<span data-ttu-id="b9a8e-130">日期</span><span class="sxs-lookup"><span data-stu-id="b9a8e-130">Date</span></span>|<span data-ttu-id="b9a8e-131">与这些统计信息关联的日期。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="b9a8e-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="b9a8e-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="b9a8e-133">Int64</span><span class="sxs-lookup"><span data-stu-id="b9a8e-133">Int64</span></span>|<span data-ttu-id="b9a8e-134">在关联日期代表用户完成的黑色和白色打印作业的数量。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-134">The number of black and white print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="b9a8e-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="b9a8e-135">completedColorJobCount</span></span>|<span data-ttu-id="b9a8e-136">Int64</span><span class="sxs-lookup"><span data-stu-id="b9a8e-136">Int64</span></span>|<span data-ttu-id="b9a8e-137">在关联日期代表用户完成的彩色打印作业的数量。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-137">The number of color print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="b9a8e-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="b9a8e-138">incompleteJobCount</span></span>|<span data-ttu-id="b9a8e-139">Int64</span><span class="sxs-lookup"><span data-stu-id="b9a8e-139">Int64</span></span>|<span data-ttu-id="b9a8e-140">在关联的日期上代表用户排队但未完成的打印作业数。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-140">The number of print jobs that were queued on behalf of the user, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b9a8e-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9a8e-141">JSON representation</span></span>

<span data-ttu-id="b9a8e-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9a8e-142">The following is a JSON representation of the resource.</span></span>

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