---
title: privilegedRoleSummary 资源类型
description: 特定角色的统计信息摘要。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 47ab49c6f91684924dab02d590427a875c1baa01
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521486"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="6b0eb-103">privilegedRoleSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b0eb-103">privilegedRoleSummary resource type</span></span>

<span data-ttu-id="6b0eb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6b0eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b0eb-105">特定角色的统计信息摘要。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-105">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="6b0eb-106">方法</span><span class="sxs-lookup"><span data-stu-id="6b0eb-106">Methods</span></span>

| <span data-ttu-id="6b0eb-107">方法</span><span class="sxs-lookup"><span data-stu-id="6b0eb-107">Method</span></span>           | <span data-ttu-id="6b0eb-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6b0eb-108">Return Type</span></span>    |<span data-ttu-id="6b0eb-109">说明</span><span class="sxs-lookup"><span data-stu-id="6b0eb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6b0eb-110">获取 privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="6b0eb-110">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="6b0eb-111">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="6b0eb-111">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="6b0eb-112">读取 privilegedRoleSummary 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-112">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6b0eb-113">属性</span><span class="sxs-lookup"><span data-stu-id="6b0eb-113">Properties</span></span>
| <span data-ttu-id="6b0eb-114">属性</span><span class="sxs-lookup"><span data-stu-id="6b0eb-114">Property</span></span>     | <span data-ttu-id="6b0eb-115">类型</span><span class="sxs-lookup"><span data-stu-id="6b0eb-115">Type</span></span>   |<span data-ttu-id="6b0eb-116">说明</span><span class="sxs-lookup"><span data-stu-id="6b0eb-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b0eb-117">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="6b0eb-117">elevatedCount</span></span>|<span data-ttu-id="6b0eb-118">int32</span><span class="sxs-lookup"><span data-stu-id="6b0eb-118">int32</span></span>|<span data-ttu-id="6b0eb-119">已分配角色并激活角色的用户数量。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-119">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="6b0eb-120">id</span><span class="sxs-lookup"><span data-stu-id="6b0eb-120">id</span></span>|<span data-ttu-id="6b0eb-121">string</span><span class="sxs-lookup"><span data-stu-id="6b0eb-121">string</span></span>| <span data-ttu-id="6b0eb-122">角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-122">The unique identifier for the role.</span></span> <span data-ttu-id="6b0eb-123">只读。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-123">Read-only.</span></span>|
|<span data-ttu-id="6b0eb-124">managedCount</span><span class="sxs-lookup"><span data-stu-id="6b0eb-124">managedCount</span></span>|<span data-ttu-id="6b0eb-125">int32</span><span class="sxs-lookup"><span data-stu-id="6b0eb-125">int32</span></span>|<span data-ttu-id="6b0eb-126">已分配角色但角色被停用的用户数量。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-126">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="6b0eb-127">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="6b0eb-127">mfaEnabled</span></span>|<span data-ttu-id="6b0eb-128">boolean</span><span class="sxs-lookup"><span data-stu-id="6b0eb-128">boolean</span></span>|<span data-ttu-id="6b0eb-129">**如此**如果角色激活需要进行 MFA。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-129">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="6b0eb-130">**假**如果角色激活不需要进行 MFA。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-130">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="6b0eb-131">状态</span><span class="sxs-lookup"><span data-stu-id="6b0eb-131">status</span></span>|<span data-ttu-id="6b0eb-132">string</span><span class="sxs-lookup"><span data-stu-id="6b0eb-132">string</span></span>| <span data-ttu-id="6b0eb-133">可取值为：`ok`、`bad`。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-133">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="6b0eb-134">值取决于（managedCount/usersCount）的比率。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-134">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="6b0eb-135">如果该比率小于预定义的阈值， `ok`则返回。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-135">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="6b0eb-136">否则， `bad`将返回。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-136">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="6b0eb-137">usersCount</span><span class="sxs-lookup"><span data-stu-id="6b0eb-137">usersCount</span></span>|<span data-ttu-id="6b0eb-138">int32</span><span class="sxs-lookup"><span data-stu-id="6b0eb-138">int32</span></span>|<span data-ttu-id="6b0eb-139">为角色分配的用户数。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-139">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b0eb-140">关系</span><span class="sxs-lookup"><span data-stu-id="6b0eb-140">Relationships</span></span>
<span data-ttu-id="6b0eb-141">无</span><span class="sxs-lookup"><span data-stu-id="6b0eb-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6b0eb-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b0eb-142">JSON representation</span></span>

<span data-ttu-id="6b0eb-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b0eb-143">Here is a JSON representation of the resource.</span></span>

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
