---
title: printUsageByUser 资源类型
description: 描述指定时间段内用户的打印活动 (usageDate) 。
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: 4b4809f77e7ceeba79ea5b7e75737fb0750cc4dc
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781227"
---
# <a name="printusagebyuser-resource-type"></a><span data-ttu-id="cef64-103">printUsageByUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="cef64-103">printUsageByUser resource type</span></span>

<span data-ttu-id="cef64-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cef64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cef64-105">描述指定时间段内用户的打印活动 (usageDate) 。</span><span class="sxs-lookup"><span data-stu-id="cef64-105">Describes print activity for a user during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="cef64-106">方法</span><span class="sxs-lookup"><span data-stu-id="cef64-106">Methods</span></span>

| <span data-ttu-id="cef64-107">方法</span><span class="sxs-lookup"><span data-stu-id="cef64-107">Method</span></span>       | <span data-ttu-id="cef64-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="cef64-108">Return Type</span></span> | <span data-ttu-id="cef64-109">说明</span><span class="sxs-lookup"><span data-stu-id="cef64-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="cef64-110">列出 (每天) </span><span class="sxs-lookup"><span data-stu-id="cef64-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagebyuser.md) | [<span data-ttu-id="cef64-111">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="cef64-111">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="cef64-112">获取每日打印使用情况摘要的列表，按用户分组。</span><span class="sxs-lookup"><span data-stu-id="cef64-112">Get a list of daily print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="cef64-113">列出 (月) </span><span class="sxs-lookup"><span data-stu-id="cef64-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagebyuser.md) | [<span data-ttu-id="cef64-114">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="cef64-114">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="cef64-115">获取按用户分组的每月打印使用情况摘要列表。</span><span class="sxs-lookup"><span data-stu-id="cef64-115">Get a list of monthly print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="cef64-116">获取</span><span class="sxs-lookup"><span data-stu-id="cef64-116">Get</span></span>](../api/printusagebyuser-get.md) | [<span data-ttu-id="cef64-117">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="cef64-117">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="cef64-118">读取 printUsageByUser 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cef64-118">Read properties and relationships of a printUsageByUser object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cef64-119">属性</span><span class="sxs-lookup"><span data-stu-id="cef64-119">Properties</span></span>
| <span data-ttu-id="cef64-120">属性</span><span class="sxs-lookup"><span data-stu-id="cef64-120">Property</span></span>     | <span data-ttu-id="cef64-121">类型</span><span class="sxs-lookup"><span data-stu-id="cef64-121">Type</span></span>        | <span data-ttu-id="cef64-122">说明</span><span class="sxs-lookup"><span data-stu-id="cef64-122">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cef64-123">id</span><span class="sxs-lookup"><span data-stu-id="cef64-123">id</span></span>|<span data-ttu-id="cef64-124">String</span><span class="sxs-lookup"><span data-stu-id="cef64-124">String</span></span>|<span data-ttu-id="cef64-125">此使用率摘要的 ID。</span><span class="sxs-lookup"><span data-stu-id="cef64-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="cef64-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="cef64-126">userPrincipalName</span></span>|<span data-ttu-id="cef64-127">String</span><span class="sxs-lookup"><span data-stu-id="cef64-127">String</span></span>|<span data-ttu-id="cef64-128">这些统计信息所代表的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="cef64-128">The UPN of the user represented by these statistics.</span></span>|
|<span data-ttu-id="cef64-129">usageDate</span><span class="sxs-lookup"><span data-stu-id="cef64-129">usageDate</span></span>|<span data-ttu-id="cef64-130">日期</span><span class="sxs-lookup"><span data-stu-id="cef64-130">Date</span></span>|<span data-ttu-id="cef64-131">与这些统计信息关联的日期。</span><span class="sxs-lookup"><span data-stu-id="cef64-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="cef64-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="cef64-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="cef64-133">Int64</span><span class="sxs-lookup"><span data-stu-id="cef64-133">Int64</span></span>|<span data-ttu-id="cef64-134">在关联的日期代表用户完成的黑白打印作业数。</span><span class="sxs-lookup"><span data-stu-id="cef64-134">The number of black and white print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="cef64-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="cef64-135">completedColorJobCount</span></span>|<span data-ttu-id="cef64-136">Int64</span><span class="sxs-lookup"><span data-stu-id="cef64-136">Int64</span></span>|<span data-ttu-id="cef64-137">在关联的日期代表用户完成的颜色打印作业数。</span><span class="sxs-lookup"><span data-stu-id="cef64-137">The number of color print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="cef64-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="cef64-138">incompleteJobCount</span></span>|<span data-ttu-id="cef64-139">Int64</span><span class="sxs-lookup"><span data-stu-id="cef64-139">Int64</span></span>|<span data-ttu-id="cef64-140">代表用户（但不在关联日期）排队的打印作业数。</span><span class="sxs-lookup"><span data-stu-id="cef64-140">The number of print jobs that were queued on behalf of the user, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cef64-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cef64-141">JSON representation</span></span>

<span data-ttu-id="cef64-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cef64-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printUsageByUser"
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
  "description": "printUsageByUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

