---
title: printUsageByUser 资源类型
description: 描述用户指定的时间段的打印活动 (usageDate) 。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: resourcePageType
ms.openlocfilehash: c478a4f9827de96d4db0da5d8533628bd8468d98
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517260"
---
# <a name="printusagebyuser-resource-type"></a><span data-ttu-id="06318-103">printUsageByUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="06318-103">printUsageByUser resource type</span></span>

<span data-ttu-id="06318-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06318-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="06318-105">描述用户指定的时间段的打印活动 (usageDate) 。</span><span class="sxs-lookup"><span data-stu-id="06318-105">Describes print activity for a user during a specified time period (usageDate).</span></span>

## <a name="methods"></a><span data-ttu-id="06318-106">Methods</span><span class="sxs-lookup"><span data-stu-id="06318-106">Methods</span></span>
|<span data-ttu-id="06318-107">方法</span><span class="sxs-lookup"><span data-stu-id="06318-107">Method</span></span>|<span data-ttu-id="06318-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="06318-108">Return type</span></span>|<span data-ttu-id="06318-109">Description</span><span class="sxs-lookup"><span data-stu-id="06318-109">Description</span></span>|
|:---|:---|:---|
| [<span data-ttu-id="06318-110">列出 (每天) </span><span class="sxs-lookup"><span data-stu-id="06318-110">List (daily)</span></span>](../api/reportroot-list-dailyprintusagebyuser.md) | [<span data-ttu-id="06318-111">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="06318-111">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="06318-112">获取每日打印使用情况摘要的列表，按用户分组。</span><span class="sxs-lookup"><span data-stu-id="06318-112">Get a list of daily print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="06318-113">列出 (每月) </span><span class="sxs-lookup"><span data-stu-id="06318-113">List (monthly)</span></span>](../api/reportroot-list-monthlyprintusagebyuser.md) | [<span data-ttu-id="06318-114">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="06318-114">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="06318-115">获取按用户分组的每月打印使用情况摘要列表。</span><span class="sxs-lookup"><span data-stu-id="06318-115">Get a list of monthly print usage summaries, grouped by user.</span></span> |
| [<span data-ttu-id="06318-116">获取</span><span class="sxs-lookup"><span data-stu-id="06318-116">Get</span></span>](../api/printusagebyuser-get.md) | [<span data-ttu-id="06318-117">printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="06318-117">printUsageByUser</span></span>](printusagebyuser.md) | <span data-ttu-id="06318-118">读取 printUsageByUser 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="06318-118">Read properties and relationships of a printUsageByUser object.</span></span> |

## <a name="properties"></a><span data-ttu-id="06318-119">属性</span><span class="sxs-lookup"><span data-stu-id="06318-119">Properties</span></span>
|<span data-ttu-id="06318-120">属性</span><span class="sxs-lookup"><span data-stu-id="06318-120">Property</span></span>|<span data-ttu-id="06318-121">类型</span><span class="sxs-lookup"><span data-stu-id="06318-121">Type</span></span>|<span data-ttu-id="06318-122">说明</span><span class="sxs-lookup"><span data-stu-id="06318-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06318-123">id</span><span class="sxs-lookup"><span data-stu-id="06318-123">id</span></span>|<span data-ttu-id="06318-124">String</span><span class="sxs-lookup"><span data-stu-id="06318-124">String</span></span>|<span data-ttu-id="06318-125">此使用率摘要的 ID。</span><span class="sxs-lookup"><span data-stu-id="06318-125">The ID of this usage summary.</span></span>|
|<span data-ttu-id="06318-126">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="06318-126">userPrincipalName</span></span>|<span data-ttu-id="06318-127">String</span><span class="sxs-lookup"><span data-stu-id="06318-127">String</span></span>|<span data-ttu-id="06318-128">这些统计信息所代表的用户的 UPN。</span><span class="sxs-lookup"><span data-stu-id="06318-128">The UPN of the user represented by these statistics.</span></span>|
|<span data-ttu-id="06318-129">usageDate</span><span class="sxs-lookup"><span data-stu-id="06318-129">usageDate</span></span>|<span data-ttu-id="06318-130">日期</span><span class="sxs-lookup"><span data-stu-id="06318-130">Date</span></span>|<span data-ttu-id="06318-131">与这些统计信息关联的日期。</span><span class="sxs-lookup"><span data-stu-id="06318-131">The date associated with these statistics.</span></span>|
|<span data-ttu-id="06318-132">completedBlackAndWhiteJobCount</span><span class="sxs-lookup"><span data-stu-id="06318-132">completedBlackAndWhiteJobCount</span></span>|<span data-ttu-id="06318-133">Int64</span><span class="sxs-lookup"><span data-stu-id="06318-133">Int64</span></span>|<span data-ttu-id="06318-134">在关联日期代表用户完成的黑白打印作业的数量。</span><span class="sxs-lookup"><span data-stu-id="06318-134">The number of black and white print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="06318-135">completedColorJobCount</span><span class="sxs-lookup"><span data-stu-id="06318-135">completedColorJobCount</span></span>|<span data-ttu-id="06318-136">Int64</span><span class="sxs-lookup"><span data-stu-id="06318-136">Int64</span></span>|<span data-ttu-id="06318-137">在关联日期代表用户完成的颜色打印作业数。</span><span class="sxs-lookup"><span data-stu-id="06318-137">The number of color print jobs completed on behalf of the user on the associated date.</span></span>|
|<span data-ttu-id="06318-138">incompleteJobCount</span><span class="sxs-lookup"><span data-stu-id="06318-138">incompleteJobCount</span></span>|<span data-ttu-id="06318-139">Int64</span><span class="sxs-lookup"><span data-stu-id="06318-139">Int64</span></span>|<span data-ttu-id="06318-140">在关联日期代表用户排队但未完成的打印作业数。</span><span class="sxs-lookup"><span data-stu-id="06318-140">The number of print jobs that were queued on behalf of the user, but not completed, on the associated date.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06318-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06318-141">JSON representation</span></span>
<span data-ttu-id="06318-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06318-142">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.printUsageByUser",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.printUsageByUser",
  "id": "String (identifier)",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": "Integer",
  "completedColorJobCount": "Integer",
  "incompleteJobCount": "Integer",
  "userPrincipalName": "String"
}
```

