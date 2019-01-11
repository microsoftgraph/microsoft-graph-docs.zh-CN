---
title: privilegedRoleSummary 资源类型
description: 为特定的角色摘要统计信息。
localization_priority: Normal
ms.openlocfilehash: b74b562a992f7795f3ae8e317608f1e370bc2a4e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858616"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="789c9-103">privilegedRoleSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="789c9-103">privilegedRoleSummary resource type</span></span>

> <span data-ttu-id="789c9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="789c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="789c9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="789c9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="789c9-106">为特定的角色摘要统计信息。</span><span class="sxs-lookup"><span data-stu-id="789c9-106">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="789c9-107">方法</span><span class="sxs-lookup"><span data-stu-id="789c9-107">Methods</span></span>

| <span data-ttu-id="789c9-108">方法</span><span class="sxs-lookup"><span data-stu-id="789c9-108">Method</span></span>           | <span data-ttu-id="789c9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="789c9-109">Return Type</span></span>    |<span data-ttu-id="789c9-110">说明</span><span class="sxs-lookup"><span data-stu-id="789c9-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="789c9-111">获取 privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="789c9-111">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="789c9-112">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="789c9-112">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="789c9-113">读取属性和 privilegedRoleSummary 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="789c9-113">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="789c9-114">属性</span><span class="sxs-lookup"><span data-stu-id="789c9-114">Properties</span></span>
| <span data-ttu-id="789c9-115">属性</span><span class="sxs-lookup"><span data-stu-id="789c9-115">Property</span></span>     | <span data-ttu-id="789c9-116">类型</span><span class="sxs-lookup"><span data-stu-id="789c9-116">Type</span></span>   |<span data-ttu-id="789c9-117">Description</span><span class="sxs-lookup"><span data-stu-id="789c9-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="789c9-118">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="789c9-118">elevatedCount</span></span>|<span data-ttu-id="789c9-119">int32</span><span class="sxs-lookup"><span data-stu-id="789c9-119">int32</span></span>|<span data-ttu-id="789c9-120">激活已分配的角色和角色的用户数。</span><span class="sxs-lookup"><span data-stu-id="789c9-120">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="789c9-121">id</span><span class="sxs-lookup"><span data-stu-id="789c9-121">id</span></span>|<span data-ttu-id="789c9-122">string</span><span class="sxs-lookup"><span data-stu-id="789c9-122">string</span></span>| <span data-ttu-id="789c9-123">角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="789c9-123">The unique identifier for the role.</span></span> <span data-ttu-id="789c9-124">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="789c9-124">Read-only.</span></span>|
|<span data-ttu-id="789c9-125">managedCount</span><span class="sxs-lookup"><span data-stu-id="789c9-125">managedCount</span></span>|<span data-ttu-id="789c9-126">int32</span><span class="sxs-lookup"><span data-stu-id="789c9-126">int32</span></span>|<span data-ttu-id="789c9-127">停用已分配的角色的用户，但该角色的数量。</span><span class="sxs-lookup"><span data-stu-id="789c9-127">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="789c9-128">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="789c9-128">mfaEnabled</span></span>|<span data-ttu-id="789c9-129">boolean</span><span class="sxs-lookup"><span data-stu-id="789c9-129">boolean</span></span>|<span data-ttu-id="789c9-130">如果为**true**的角色激活需要 MFA。</span><span class="sxs-lookup"><span data-stu-id="789c9-130">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="789c9-131">**false**如果角色激活不需要 MFA。</span><span class="sxs-lookup"><span data-stu-id="789c9-131">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="789c9-132">status</span><span class="sxs-lookup"><span data-stu-id="789c9-132">status</span></span>|<span data-ttu-id="789c9-133">string</span><span class="sxs-lookup"><span data-stu-id="789c9-133">string</span></span>| <span data-ttu-id="789c9-134">可取值为：`ok`、`bad`。</span><span class="sxs-lookup"><span data-stu-id="789c9-134">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="789c9-135">值取决于的比率 (managedCount / usersCount)。</span><span class="sxs-lookup"><span data-stu-id="789c9-135">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="789c9-136">如果此比率小于预定义的阈值，`ok`返回。</span><span class="sxs-lookup"><span data-stu-id="789c9-136">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="789c9-137">否则为`bad`返回。</span><span class="sxs-lookup"><span data-stu-id="789c9-137">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="789c9-138">usersCount</span><span class="sxs-lookup"><span data-stu-id="789c9-138">usersCount</span></span>|<span data-ttu-id="789c9-139">int32</span><span class="sxs-lookup"><span data-stu-id="789c9-139">int32</span></span>|<span data-ttu-id="789c9-140">与角色分配的用户数。</span><span class="sxs-lookup"><span data-stu-id="789c9-140">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="789c9-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="789c9-141">Relationships</span></span>
<span data-ttu-id="789c9-142">无</span><span class="sxs-lookup"><span data-stu-id="789c9-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="789c9-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="789c9-143">JSON representation</span></span>

<span data-ttu-id="789c9-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="789c9-144">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleSummary resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
