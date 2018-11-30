---
title: privilegedRoleSummary 资源类型
description: 为特定的角色摘要统计信息。
ms.openlocfilehash: f6c66433651eff188ce6fdaa07c2422d3bb6e0ce
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047984"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="34434-103">privilegedRoleSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="34434-103">privilegedRoleSummary resource type</span></span>

> <span data-ttu-id="34434-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="34434-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34434-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="34434-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34434-106">为特定的角色摘要统计信息。</span><span class="sxs-lookup"><span data-stu-id="34434-106">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="34434-107">方法</span><span class="sxs-lookup"><span data-stu-id="34434-107">Methods</span></span>

| <span data-ttu-id="34434-108">方法</span><span class="sxs-lookup"><span data-stu-id="34434-108">Method</span></span>           | <span data-ttu-id="34434-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="34434-109">Return Type</span></span>    |<span data-ttu-id="34434-110">说明</span><span class="sxs-lookup"><span data-stu-id="34434-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="34434-111">获取 privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="34434-111">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="34434-112">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="34434-112">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="34434-113">读取属性和 privilegedRoleSummary 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="34434-113">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="34434-114">属性</span><span class="sxs-lookup"><span data-stu-id="34434-114">Properties</span></span>
| <span data-ttu-id="34434-115">属性</span><span class="sxs-lookup"><span data-stu-id="34434-115">Property</span></span>     | <span data-ttu-id="34434-116">类型</span><span class="sxs-lookup"><span data-stu-id="34434-116">Type</span></span>   |<span data-ttu-id="34434-117">说明</span><span class="sxs-lookup"><span data-stu-id="34434-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34434-118">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="34434-118">elevatedCount</span></span>|<span data-ttu-id="34434-119">int32</span><span class="sxs-lookup"><span data-stu-id="34434-119">int32</span></span>|<span data-ttu-id="34434-120">激活已分配的角色和角色的用户数。</span><span class="sxs-lookup"><span data-stu-id="34434-120">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="34434-121">id</span><span class="sxs-lookup"><span data-stu-id="34434-121">id</span></span>|<span data-ttu-id="34434-122">string</span><span class="sxs-lookup"><span data-stu-id="34434-122">string</span></span>| <span data-ttu-id="34434-123">角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="34434-123">The unique identifier for the role.</span></span> <span data-ttu-id="34434-124">只读。</span><span class="sxs-lookup"><span data-stu-id="34434-124">Read-only.</span></span>|
|<span data-ttu-id="34434-125">managedCount</span><span class="sxs-lookup"><span data-stu-id="34434-125">managedCount</span></span>|<span data-ttu-id="34434-126">int32</span><span class="sxs-lookup"><span data-stu-id="34434-126">int32</span></span>|<span data-ttu-id="34434-127">停用已分配的角色的用户，但该角色的数量。</span><span class="sxs-lookup"><span data-stu-id="34434-127">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="34434-128">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="34434-128">mfaEnabled</span></span>|<span data-ttu-id="34434-129">boolean</span><span class="sxs-lookup"><span data-stu-id="34434-129">boolean</span></span>|<span data-ttu-id="34434-130">如果为**true**的角色激活需要 MFA。</span><span class="sxs-lookup"><span data-stu-id="34434-130">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="34434-131">**false**如果角色激活不需要 MFA。</span><span class="sxs-lookup"><span data-stu-id="34434-131">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="34434-132">status</span><span class="sxs-lookup"><span data-stu-id="34434-132">status</span></span>|<span data-ttu-id="34434-133">string</span><span class="sxs-lookup"><span data-stu-id="34434-133">string</span></span>| <span data-ttu-id="34434-134">可取值为：`ok`、`bad`。</span><span class="sxs-lookup"><span data-stu-id="34434-134">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="34434-135">值取决于的比率 (managedCount / usersCount)。</span><span class="sxs-lookup"><span data-stu-id="34434-135">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="34434-136">如果此比率小于预定义的阈值，`ok`返回。</span><span class="sxs-lookup"><span data-stu-id="34434-136">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="34434-137">否则为`bad`返回。</span><span class="sxs-lookup"><span data-stu-id="34434-137">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="34434-138">usersCount</span><span class="sxs-lookup"><span data-stu-id="34434-138">usersCount</span></span>|<span data-ttu-id="34434-139">int32</span><span class="sxs-lookup"><span data-stu-id="34434-139">int32</span></span>|<span data-ttu-id="34434-140">与角色分配的用户数。</span><span class="sxs-lookup"><span data-stu-id="34434-140">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="34434-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="34434-141">Relationships</span></span>
<span data-ttu-id="34434-142">无</span><span class="sxs-lookup"><span data-stu-id="34434-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="34434-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34434-143">JSON representation</span></span>

<span data-ttu-id="34434-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34434-144">Here is a JSON representation of the resource.</span></span>

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