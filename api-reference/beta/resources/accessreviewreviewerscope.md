---
title: accessReviewReviewerScope 资源类型
description: 表示将审阅访问评审的人。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 68f353b81b6a14292828d82929a0eeac81d67bc5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469155"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="b297a-103">accessReviewReviewerScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="b297a-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="b297a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b297a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="b297a-105">accessReviewReviewerScope 定义谁将审阅 [accessReviewScheduleDefinition 的实例](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="b297a-105">The accessReviewReviewerScope defines who will review instances of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="b297a-106">这表示为 OData 查询，它允许将审阅者指定为用户的静态列表 (即特定用户、组所有者、组成员) 或动态 (，即每个用户都由其经理) 审阅的情况。</span><span class="sxs-lookup"><span data-stu-id="b297a-106">This is expressed as an OData query, which allows reviewers to be specified both as a static list of users (i.e., specific users, group owners, group members) or dynamically (i.e., the case where every user is reviewed by their manager).</span></span> <span data-ttu-id="b297a-107">若要创建自审阅 (用户查看自己的访问权限) ，请不要在 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 创建时提供审阅者。</span><span class="sxs-lookup"><span data-stu-id="b297a-107">To create a self-review (where users review their own access), do not provide reviewers on [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) creation.</span></span>

<span data-ttu-id="b297a-108">继承自 [accessReviewScope](../resources/accessreviewscope.md)。</span><span class="sxs-lookup"><span data-stu-id="b297a-108">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b297a-109">属性</span><span class="sxs-lookup"><span data-stu-id="b297a-109">Properties</span></span>
| <span data-ttu-id="b297a-110">属性</span><span class="sxs-lookup"><span data-stu-id="b297a-110">Property</span></span> | <span data-ttu-id="b297a-111">类型</span><span class="sxs-lookup"><span data-stu-id="b297a-111">Type</span></span> | <span data-ttu-id="b297a-112">说明</span><span class="sxs-lookup"><span data-stu-id="b297a-112">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="b297a-113">查询</span><span class="sxs-lookup"><span data-stu-id="b297a-113">query</span></span> | <span data-ttu-id="b297a-114">String</span><span class="sxs-lookup"><span data-stu-id="b297a-114">String</span></span> | <span data-ttu-id="b297a-115">用于指定审阅者的查询。</span><span class="sxs-lookup"><span data-stu-id="b297a-115">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="b297a-116">有关示例，请参阅表。</span><span class="sxs-lookup"><span data-stu-id="b297a-116">See table for examples.</span></span> |
| <span data-ttu-id="b297a-117">queryType</span><span class="sxs-lookup"><span data-stu-id="b297a-117">queryType</span></span> | <span data-ttu-id="b297a-118">String</span><span class="sxs-lookup"><span data-stu-id="b297a-118">String</span></span> | <span data-ttu-id="b297a-119">查询的类型。</span><span class="sxs-lookup"><span data-stu-id="b297a-119">The type of query.</span></span> <span data-ttu-id="b297a-120">示例包括 `MicrosoftGraph` `ARM` 和 。</span><span class="sxs-lookup"><span data-stu-id="b297a-120">Examples include `MicrosoftGraph` and `ARM`.</span></span> |
| <span data-ttu-id="b297a-121">queryRoot</span><span class="sxs-lookup"><span data-stu-id="b297a-121">queryRoot</span></span> | <span data-ttu-id="b297a-122">String</span><span class="sxs-lookup"><span data-stu-id="b297a-122">String</span></span> | <span data-ttu-id="b297a-123">在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。</span><span class="sxs-lookup"><span data-stu-id="b297a-123">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="b297a-124">此属性仅在指定了相对查询 (，即 ./manager) 是必需的。</span><span class="sxs-lookup"><span data-stu-id="b297a-124">This property is only required if a relative query (i.e., ./manager) is specified.</span></span> |

### <a name="supported-queries-for-accessreviewreviewerscope"></a><span data-ttu-id="b297a-125">accessReviewReviewerScope 支持的查询</span><span class="sxs-lookup"><span data-stu-id="b297a-125">Supported queries for accessReviewReviewerScope</span></span>

|<span data-ttu-id="b297a-126">方案</span><span class="sxs-lookup"><span data-stu-id="b297a-126">Scenario</span></span>| <span data-ttu-id="b297a-127">查询</span><span class="sxs-lookup"><span data-stu-id="b297a-127">query</span></span> | <span data-ttu-id="b297a-128">queryType</span><span class="sxs-lookup"><span data-stu-id="b297a-128">queryType</span></span> | <span data-ttu-id="b297a-129">queryRoot</span><span class="sxs-lookup"><span data-stu-id="b297a-129">queryRoot</span></span> |
|--|--|--|--|
| <span data-ttu-id="b297a-130">作为审阅者的组所有者</span><span class="sxs-lookup"><span data-stu-id="b297a-130">Group owner as reviewer</span></span> | <span data-ttu-id="b297a-131">/groups/{group id}/owners</span><span class="sxs-lookup"><span data-stu-id="b297a-131">/groups/{group id}/owners</span></span> |<span data-ttu-id="b297a-132">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="b297a-132">MicrosoftGraph</span></span>||
| <span data-ttu-id="b297a-133">作为审阅者的特定用户</span><span class="sxs-lookup"><span data-stu-id="b297a-133">Specific user as reviewer</span></span> | <span data-ttu-id="b297a-134">/users/{user id}</span><span class="sxs-lookup"><span data-stu-id="b297a-134">/users/{user id}</span></span> |<span data-ttu-id="b297a-135">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="b297a-135">MicrosoftGraph</span></span>||
| <span data-ttu-id="b297a-136">被审阅为审阅者的用户的经理</span><span class="sxs-lookup"><span data-stu-id="b297a-136">Manager of user being reviewed as reviewer</span></span> | <span data-ttu-id="b297a-137">./manager</span><span class="sxs-lookup"><span data-stu-id="b297a-137">./manager</span></span> | <span data-ttu-id="b297a-138">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="b297a-138">MicrosoftGraph</span></span> |<span data-ttu-id="b297a-139">决策</span><span class="sxs-lookup"><span data-stu-id="b297a-139">decisions</span></span>|
| <span data-ttu-id="b297a-140">自我审阅</span><span class="sxs-lookup"><span data-stu-id="b297a-140">Self Review</span></span> | <span data-ttu-id="b297a-141">空列表 (没有审阅者) </span><span class="sxs-lookup"><span data-stu-id="b297a-141">Empty list(No reviewers)</span></span> | <span data-ttu-id="b297a-142">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="b297a-142">MicrosoftGraph</span></span>  |


## <a name="relationships"></a><span data-ttu-id="b297a-143">关系</span><span class="sxs-lookup"><span data-stu-id="b297a-143">Relationships</span></span>
<span data-ttu-id="b297a-144">无。</span><span class="sxs-lookup"><span data-stu-id="b297a-144">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b297a-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b297a-145">JSON representation</span></span>
<span data-ttu-id="b297a-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b297a-146">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewReviewerScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewReviewerScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewReviewerScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
