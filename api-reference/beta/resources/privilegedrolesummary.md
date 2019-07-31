---
title: privilegedRoleSummary 资源类型
description: 特定角色的统计信息摘要。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 30c9cfb93f8d20d30ad86d0f36019e87eae0ab65
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965715"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="9299e-103">privilegedRoleSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="9299e-103">privilegedRoleSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9299e-104">特定角色的统计信息摘要。</span><span class="sxs-lookup"><span data-stu-id="9299e-104">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="9299e-105">方法</span><span class="sxs-lookup"><span data-stu-id="9299e-105">Methods</span></span>

| <span data-ttu-id="9299e-106">方法</span><span class="sxs-lookup"><span data-stu-id="9299e-106">Method</span></span>           | <span data-ttu-id="9299e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="9299e-107">Return Type</span></span>    |<span data-ttu-id="9299e-108">说明</span><span class="sxs-lookup"><span data-stu-id="9299e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9299e-109">获取 privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="9299e-109">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="9299e-110">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="9299e-110">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="9299e-111">读取 privilegedRoleSummary 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9299e-111">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9299e-112">属性</span><span class="sxs-lookup"><span data-stu-id="9299e-112">Properties</span></span>
| <span data-ttu-id="9299e-113">属性</span><span class="sxs-lookup"><span data-stu-id="9299e-113">Property</span></span>     | <span data-ttu-id="9299e-114">类型</span><span class="sxs-lookup"><span data-stu-id="9299e-114">Type</span></span>   |<span data-ttu-id="9299e-115">说明</span><span class="sxs-lookup"><span data-stu-id="9299e-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9299e-116">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="9299e-116">elevatedCount</span></span>|<span data-ttu-id="9299e-117">int32</span><span class="sxs-lookup"><span data-stu-id="9299e-117">int32</span></span>|<span data-ttu-id="9299e-118">已分配角色并激活角色的用户数量。</span><span class="sxs-lookup"><span data-stu-id="9299e-118">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="9299e-119">id</span><span class="sxs-lookup"><span data-stu-id="9299e-119">id</span></span>|<span data-ttu-id="9299e-120">string</span><span class="sxs-lookup"><span data-stu-id="9299e-120">string</span></span>| <span data-ttu-id="9299e-121">角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="9299e-121">The unique identifier for the role.</span></span> <span data-ttu-id="9299e-122">只读。</span><span class="sxs-lookup"><span data-stu-id="9299e-122">Read-only.</span></span>|
|<span data-ttu-id="9299e-123">managedCount</span><span class="sxs-lookup"><span data-stu-id="9299e-123">managedCount</span></span>|<span data-ttu-id="9299e-124">int32</span><span class="sxs-lookup"><span data-stu-id="9299e-124">int32</span></span>|<span data-ttu-id="9299e-125">已分配角色但角色被停用的用户数量。</span><span class="sxs-lookup"><span data-stu-id="9299e-125">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="9299e-126">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="9299e-126">mfaEnabled</span></span>|<span data-ttu-id="9299e-127">boolean</span><span class="sxs-lookup"><span data-stu-id="9299e-127">boolean</span></span>|<span data-ttu-id="9299e-128">**如此**如果角色激活需要进行 MFA。</span><span class="sxs-lookup"><span data-stu-id="9299e-128">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="9299e-129">**假**如果角色激活不需要进行 MFA。</span><span class="sxs-lookup"><span data-stu-id="9299e-129">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="9299e-130">状态</span><span class="sxs-lookup"><span data-stu-id="9299e-130">status</span></span>|<span data-ttu-id="9299e-131">string</span><span class="sxs-lookup"><span data-stu-id="9299e-131">string</span></span>| <span data-ttu-id="9299e-132">可取值为：`ok`、`bad`。</span><span class="sxs-lookup"><span data-stu-id="9299e-132">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="9299e-133">值取决于 (managedCount/usersCount) 的比率。</span><span class="sxs-lookup"><span data-stu-id="9299e-133">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="9299e-134">如果该比率小于预定义的阈值, `ok`则返回。</span><span class="sxs-lookup"><span data-stu-id="9299e-134">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="9299e-135">否则, `bad`将返回。</span><span class="sxs-lookup"><span data-stu-id="9299e-135">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="9299e-136">usersCount</span><span class="sxs-lookup"><span data-stu-id="9299e-136">usersCount</span></span>|<span data-ttu-id="9299e-137">int32</span><span class="sxs-lookup"><span data-stu-id="9299e-137">int32</span></span>|<span data-ttu-id="9299e-138">为角色分配的用户数。</span><span class="sxs-lookup"><span data-stu-id="9299e-138">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9299e-139">关系</span><span class="sxs-lookup"><span data-stu-id="9299e-139">Relationships</span></span>
<span data-ttu-id="9299e-140">无</span><span class="sxs-lookup"><span data-stu-id="9299e-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9299e-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9299e-141">JSON representation</span></span>

<span data-ttu-id="9299e-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9299e-142">Here is a JSON representation of the resource.</span></span>

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
