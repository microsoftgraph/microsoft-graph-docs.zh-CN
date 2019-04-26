---
title: privilegedRoleSummary 资源类型
description: 特定角色的统计信息摘要。
localization_priority: Normal
ms.openlocfilehash: 3e7b447f63c5f8545021508ae2dc137bef845210
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344260"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="645aa-103">privilegedRoleSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="645aa-103">privilegedRoleSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="645aa-104">特定角色的统计信息摘要。</span><span class="sxs-lookup"><span data-stu-id="645aa-104">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="645aa-105">方法</span><span class="sxs-lookup"><span data-stu-id="645aa-105">Methods</span></span>

| <span data-ttu-id="645aa-106">方法</span><span class="sxs-lookup"><span data-stu-id="645aa-106">Method</span></span>           | <span data-ttu-id="645aa-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="645aa-107">Return Type</span></span>    |<span data-ttu-id="645aa-108">说明</span><span class="sxs-lookup"><span data-stu-id="645aa-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="645aa-109">获取 privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="645aa-109">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="645aa-110">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="645aa-110">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="645aa-111">读取 privilegedRoleSummary 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="645aa-111">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="645aa-112">属性</span><span class="sxs-lookup"><span data-stu-id="645aa-112">Properties</span></span>
| <span data-ttu-id="645aa-113">属性</span><span class="sxs-lookup"><span data-stu-id="645aa-113">Property</span></span>     | <span data-ttu-id="645aa-114">类型</span><span class="sxs-lookup"><span data-stu-id="645aa-114">Type</span></span>   |<span data-ttu-id="645aa-115">说明</span><span class="sxs-lookup"><span data-stu-id="645aa-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="645aa-116">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="645aa-116">elevatedCount</span></span>|<span data-ttu-id="645aa-117">时会</span><span class="sxs-lookup"><span data-stu-id="645aa-117">int32</span></span>|<span data-ttu-id="645aa-118">已分配角色并激活角色的用户数量。</span><span class="sxs-lookup"><span data-stu-id="645aa-118">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="645aa-119">id</span><span class="sxs-lookup"><span data-stu-id="645aa-119">id</span></span>|<span data-ttu-id="645aa-120">string</span><span class="sxs-lookup"><span data-stu-id="645aa-120">string</span></span>| <span data-ttu-id="645aa-121">角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="645aa-121">The unique identifier for the role.</span></span> <span data-ttu-id="645aa-122">只读。</span><span class="sxs-lookup"><span data-stu-id="645aa-122">Read-only.</span></span>|
|<span data-ttu-id="645aa-123">managedCount</span><span class="sxs-lookup"><span data-stu-id="645aa-123">managedCount</span></span>|<span data-ttu-id="645aa-124">时会</span><span class="sxs-lookup"><span data-stu-id="645aa-124">int32</span></span>|<span data-ttu-id="645aa-125">已分配角色但角色被停用的用户数量。</span><span class="sxs-lookup"><span data-stu-id="645aa-125">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="645aa-126">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="645aa-126">mfaEnabled</span></span>|<span data-ttu-id="645aa-127">boolean</span><span class="sxs-lookup"><span data-stu-id="645aa-127">boolean</span></span>|<span data-ttu-id="645aa-128">**如此**如果角色激活需要进行 MFA。</span><span class="sxs-lookup"><span data-stu-id="645aa-128">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="645aa-129">**假**如果角色激活不需要进行 MFA。</span><span class="sxs-lookup"><span data-stu-id="645aa-129">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="645aa-130">状态</span><span class="sxs-lookup"><span data-stu-id="645aa-130">status</span></span>|<span data-ttu-id="645aa-131">string</span><span class="sxs-lookup"><span data-stu-id="645aa-131">string</span></span>| <span data-ttu-id="645aa-132">可取值为：`ok`、`bad`。</span><span class="sxs-lookup"><span data-stu-id="645aa-132">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="645aa-133">值取决于 (managedCount/usersCount) 的比率。</span><span class="sxs-lookup"><span data-stu-id="645aa-133">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="645aa-134">如果该比率小于预定义的阈值, `ok`则返回。</span><span class="sxs-lookup"><span data-stu-id="645aa-134">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="645aa-135">否则, `bad`将返回。</span><span class="sxs-lookup"><span data-stu-id="645aa-135">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="645aa-136">usersCount</span><span class="sxs-lookup"><span data-stu-id="645aa-136">usersCount</span></span>|<span data-ttu-id="645aa-137">时会</span><span class="sxs-lookup"><span data-stu-id="645aa-137">int32</span></span>|<span data-ttu-id="645aa-138">为角色分配的用户数。</span><span class="sxs-lookup"><span data-stu-id="645aa-138">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="645aa-139">关系</span><span class="sxs-lookup"><span data-stu-id="645aa-139">Relationships</span></span>
<span data-ttu-id="645aa-140">无</span><span class="sxs-lookup"><span data-stu-id="645aa-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="645aa-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="645aa-141">JSON representation</span></span>

<span data-ttu-id="645aa-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="645aa-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.privilegedRoleSummary"
}-->

```json
{
  "elevatedCount": 1024,
  "id": "string (identifier)",
  "managedCount": 1024,
  "mfaEnabled": true,
  "status": "string",
  "usersCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
