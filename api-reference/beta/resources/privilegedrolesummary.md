---
title: privilegedRoleSummary 资源类型
description: 为特定的角色摘要统计信息。
localization_priority: Normal
ms.openlocfilehash: 2ed34f556f52c41729bfa108fbb6eb0c608f6b67
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513737"
---
# <a name="privilegedrolesummary-resource-type"></a><span data-ttu-id="c541e-103">privilegedRoleSummary 资源类型</span><span class="sxs-lookup"><span data-stu-id="c541e-103">privilegedRoleSummary resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c541e-104">为特定的角色摘要统计信息。</span><span class="sxs-lookup"><span data-stu-id="c541e-104">The statistics summary for a particular role.</span></span>


## <a name="methods"></a><span data-ttu-id="c541e-105">方法</span><span class="sxs-lookup"><span data-stu-id="c541e-105">Methods</span></span>

| <span data-ttu-id="c541e-106">方法</span><span class="sxs-lookup"><span data-stu-id="c541e-106">Method</span></span>           | <span data-ttu-id="c541e-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="c541e-107">Return Type</span></span>    |<span data-ttu-id="c541e-108">说明</span><span class="sxs-lookup"><span data-stu-id="c541e-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c541e-109">获取 privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="c541e-109">Get privilegedRoleSummary</span></span>](../api/privilegedrolesummary-get.md) | [<span data-ttu-id="c541e-110">privilegedRoleSummary</span><span class="sxs-lookup"><span data-stu-id="c541e-110">privilegedRoleSummary</span></span>](privilegedrolesummary.md) |<span data-ttu-id="c541e-111">读取属性和 privilegedRoleSummary 对象的关系。</span><span class="sxs-lookup"><span data-stu-id="c541e-111">Read properties and relationships of privilegedRoleSummary object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c541e-112">属性</span><span class="sxs-lookup"><span data-stu-id="c541e-112">Properties</span></span>
| <span data-ttu-id="c541e-113">属性</span><span class="sxs-lookup"><span data-stu-id="c541e-113">Property</span></span>     | <span data-ttu-id="c541e-114">类型</span><span class="sxs-lookup"><span data-stu-id="c541e-114">Type</span></span>   |<span data-ttu-id="c541e-115">说明</span><span class="sxs-lookup"><span data-stu-id="c541e-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c541e-116">elevatedCount</span><span class="sxs-lookup"><span data-stu-id="c541e-116">elevatedCount</span></span>|<span data-ttu-id="c541e-117">int32</span><span class="sxs-lookup"><span data-stu-id="c541e-117">int32</span></span>|<span data-ttu-id="c541e-118">激活已分配的角色和角色的用户数。</span><span class="sxs-lookup"><span data-stu-id="c541e-118">The number of users that have the role assigned and the role is activated.</span></span>|
|<span data-ttu-id="c541e-119">id</span><span class="sxs-lookup"><span data-stu-id="c541e-119">id</span></span>|<span data-ttu-id="c541e-120">string</span><span class="sxs-lookup"><span data-stu-id="c541e-120">string</span></span>| <span data-ttu-id="c541e-121">角色的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c541e-121">The unique identifier for the role.</span></span> <span data-ttu-id="c541e-122">只读。</span><span class="sxs-lookup"><span data-stu-id="c541e-122">Read-only.</span></span>|
|<span data-ttu-id="c541e-123">managedCount</span><span class="sxs-lookup"><span data-stu-id="c541e-123">managedCount</span></span>|<span data-ttu-id="c541e-124">int32</span><span class="sxs-lookup"><span data-stu-id="c541e-124">int32</span></span>|<span data-ttu-id="c541e-125">停用已分配的角色的用户，但该角色的数量。</span><span class="sxs-lookup"><span data-stu-id="c541e-125">The number of users that have the role assigned but the role is deactivated.</span></span>|
|<span data-ttu-id="c541e-126">mfaEnabled</span><span class="sxs-lookup"><span data-stu-id="c541e-126">mfaEnabled</span></span>|<span data-ttu-id="c541e-127">布尔</span><span class="sxs-lookup"><span data-stu-id="c541e-127">boolean</span></span>|<span data-ttu-id="c541e-128">如果为**true**的角色激活需要 MFA。</span><span class="sxs-lookup"><span data-stu-id="c541e-128">**true** if the role activation requires MFA.</span></span> <span data-ttu-id="c541e-129">**false**如果角色激活不需要 MFA。</span><span class="sxs-lookup"><span data-stu-id="c541e-129">**false** if the role activation doesn't require MFA.</span></span>|
|<span data-ttu-id="c541e-130">status</span><span class="sxs-lookup"><span data-stu-id="c541e-130">status</span></span>|<span data-ttu-id="c541e-131">string</span><span class="sxs-lookup"><span data-stu-id="c541e-131">string</span></span>| <span data-ttu-id="c541e-132">可取值为：`ok`、`bad`。</span><span class="sxs-lookup"><span data-stu-id="c541e-132">Possible values are: `ok`, `bad`.</span></span> <span data-ttu-id="c541e-133">值取决于的比率 (managedCount / usersCount)。</span><span class="sxs-lookup"><span data-stu-id="c541e-133">The value depends on the ratio of (managedCount / usersCount).</span></span> <span data-ttu-id="c541e-134">如果此比率小于预定义的阈值，`ok`返回。</span><span class="sxs-lookup"><span data-stu-id="c541e-134">If the ratio is less than a predefined threshold, `ok` is returned.</span></span> <span data-ttu-id="c541e-135">否则为`bad`返回。</span><span class="sxs-lookup"><span data-stu-id="c541e-135">Otherwise, `bad` is returned.</span></span>|
|<span data-ttu-id="c541e-136">usersCount</span><span class="sxs-lookup"><span data-stu-id="c541e-136">usersCount</span></span>|<span data-ttu-id="c541e-137">int32</span><span class="sxs-lookup"><span data-stu-id="c541e-137">int32</span></span>|<span data-ttu-id="c541e-138">与角色分配的用户数。</span><span class="sxs-lookup"><span data-stu-id="c541e-138">The number of users that are assigned with the role.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c541e-139">关系</span><span class="sxs-lookup"><span data-stu-id="c541e-139">Relationships</span></span>
<span data-ttu-id="c541e-140">无</span><span class="sxs-lookup"><span data-stu-id="c541e-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c541e-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c541e-141">JSON representation</span></span>

<span data-ttu-id="c541e-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c541e-142">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/privilegedrolesummary.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
