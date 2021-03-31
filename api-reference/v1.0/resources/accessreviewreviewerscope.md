---
title: accessReviewReviewerScope 资源类型
description: 表示将审阅访问评审的人。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 55f881ff1bcb1b08cc66938fd8a7b4d28f540687
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469544"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="deaea-103">accessReviewReviewerScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="deaea-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="deaea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deaea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="deaea-105">accessReviewReviewerScope 定义在 [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 中指定的审阅 [appConsentRequests](../resources/appconsentrequest.md) 和 [userConsentRequests 的用户](../resources/appconsentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="deaea-105">The accessReviewReviewerScope defines who is specified in the [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) to review [appConsentRequests](../resources/appconsentrequest.md) and [userConsentRequests](../resources/appconsentrequest.md).</span></span> <span data-ttu-id="deaea-106">这表示为 OData 查询，它允许将审阅者指定为用户的静态列表 (即特定用户、组所有者、组成员) 或动态 (，即每个用户都由其经理) 审阅的情况。</span><span class="sxs-lookup"><span data-stu-id="deaea-106">This is expressed as an OData query, which allows reviewers to be specified both as a static list of users (i.e., specific users, group owners, group members) or dynamically (i.e., the case where every user is reviewed by their manager).</span></span>

## <a name="properties"></a><span data-ttu-id="deaea-107">属性</span><span class="sxs-lookup"><span data-stu-id="deaea-107">Properties</span></span>

|<span data-ttu-id="deaea-108">属性</span><span class="sxs-lookup"><span data-stu-id="deaea-108">Property</span></span>|<span data-ttu-id="deaea-109">类型</span><span class="sxs-lookup"><span data-stu-id="deaea-109">Type</span></span>|<span data-ttu-id="deaea-110">说明</span><span class="sxs-lookup"><span data-stu-id="deaea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="deaea-111">查询</span><span class="sxs-lookup"><span data-stu-id="deaea-111">query</span></span>|<span data-ttu-id="deaea-112">String</span><span class="sxs-lookup"><span data-stu-id="deaea-112">String</span></span>|<span data-ttu-id="deaea-113">用于指定审阅者的查询。</span><span class="sxs-lookup"><span data-stu-id="deaea-113">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="deaea-114">有关示例，请参阅表。</span><span class="sxs-lookup"><span data-stu-id="deaea-114">See table for examples.</span></span> |
|<span data-ttu-id="deaea-115">queryRoot</span><span class="sxs-lookup"><span data-stu-id="deaea-115">queryRoot</span></span>|<span data-ttu-id="deaea-116">String</span><span class="sxs-lookup"><span data-stu-id="deaea-116">String</span></span>|<span data-ttu-id="deaea-117">查询的类型。</span><span class="sxs-lookup"><span data-stu-id="deaea-117">The type of query.</span></span> <span data-ttu-id="deaea-118">示例包括 `MicrosoftGraph` `ARM` 和 。</span><span class="sxs-lookup"><span data-stu-id="deaea-118">Examples include `MicrosoftGraph` and `ARM`.</span></span>|
|<span data-ttu-id="deaea-119">queryType</span><span class="sxs-lookup"><span data-stu-id="deaea-119">queryType</span></span>|<span data-ttu-id="deaea-120">String</span><span class="sxs-lookup"><span data-stu-id="deaea-120">String</span></span>|<span data-ttu-id="deaea-121">在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。</span><span class="sxs-lookup"><span data-stu-id="deaea-121">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="deaea-122">此属性仅在指定了相对查询 (，即) `./manager` 时是必需的。</span><span class="sxs-lookup"><span data-stu-id="deaea-122">This property is only required if a relative query (i.e., `./manager`) is specified.</span></span>|

### <a name="supported-queries-for-accessreviewreviewerscope"></a><span data-ttu-id="deaea-123">accessReviewReviewerScope 支持的查询</span><span class="sxs-lookup"><span data-stu-id="deaea-123">Supported queries for accessReviewReviewerScope</span></span>

|<span data-ttu-id="deaea-124">方案</span><span class="sxs-lookup"><span data-stu-id="deaea-124">Scenario</span></span>| <span data-ttu-id="deaea-125">查询</span><span class="sxs-lookup"><span data-stu-id="deaea-125">query</span></span> | <span data-ttu-id="deaea-126">queryType</span><span class="sxs-lookup"><span data-stu-id="deaea-126">queryType</span></span> | <span data-ttu-id="deaea-127">queryRoot</span><span class="sxs-lookup"><span data-stu-id="deaea-127">queryRoot</span></span> |
|--|--|--|--|
| <span data-ttu-id="deaea-128">作为审阅者的组所有者</span><span class="sxs-lookup"><span data-stu-id="deaea-128">Group owner as reviewer</span></span> | <span data-ttu-id="deaea-129">/groups/{group id}/owners</span><span class="sxs-lookup"><span data-stu-id="deaea-129">/groups/{group id}/owners</span></span> |<span data-ttu-id="deaea-130">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="deaea-130">MicrosoftGraph</span></span>||
| <span data-ttu-id="deaea-131">作为审阅者的特定用户</span><span class="sxs-lookup"><span data-stu-id="deaea-131">Specific user as reviewer</span></span> | <span data-ttu-id="deaea-132">/users/{user id}</span><span class="sxs-lookup"><span data-stu-id="deaea-132">/users/{user id}</span></span> |<span data-ttu-id="deaea-133">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="deaea-133">MicrosoftGraph</span></span>||
| <span data-ttu-id="deaea-134">被审阅为审阅者的用户的经理</span><span class="sxs-lookup"><span data-stu-id="deaea-134">Manager of user being reviewed as reviewer</span></span> | <span data-ttu-id="deaea-135">./manager</span><span class="sxs-lookup"><span data-stu-id="deaea-135">./manager</span></span> | <span data-ttu-id="deaea-136">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="deaea-136">MicrosoftGraph</span></span> |<span data-ttu-id="deaea-137">决策</span><span class="sxs-lookup"><span data-stu-id="deaea-137">decisions</span></span>|

## <a name="relationships"></a><span data-ttu-id="deaea-138">关系</span><span class="sxs-lookup"><span data-stu-id="deaea-138">Relationships</span></span>

<span data-ttu-id="deaea-139">无。</span><span class="sxs-lookup"><span data-stu-id="deaea-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="deaea-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="deaea-140">JSON representation</span></span>

<span data-ttu-id="deaea-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="deaea-141">The following is a JSON representation of the resource.</span></span>
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
