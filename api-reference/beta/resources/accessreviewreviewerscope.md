---
title: accessReviewReviewerScope 资源类型
description: 代表将审阅访问评审的人。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7c8a0644699daf7e204226d89bdd6cab6048888d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133488"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="78f56-103">accessReviewReviewerScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="78f56-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="78f56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78f56-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78f56-105">accessReviewReviewerScope 定义谁将审阅 [accessReviewScheduleDefinition 的实例](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="78f56-105">The accessReviewReviewerScope defines who will review instances of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="78f56-106">这表示为 OData 查询，它允许将审阅者指定为用户的静态列表 (即特定用户、组所有者、组成员) 或动态 (，即每个用户都由其经理) 审阅的情况。</span><span class="sxs-lookup"><span data-stu-id="78f56-106">This is expressed as an OData query, which allows reviewers to be specified both as a static list of users (i.e., specific users, group owners, group members) or dynamically (i.e., the case where every user is reviewed by their manager).</span></span> <span data-ttu-id="78f56-107">若要创建自 (查看自己的访问权限的自) ，请不要在 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 创建时提供审阅者。</span><span class="sxs-lookup"><span data-stu-id="78f56-107">To create a self-review (where users review their own access), do not provide reviewers on [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) creation.</span></span>


## <a name="properties"></a><span data-ttu-id="78f56-108">属性</span><span class="sxs-lookup"><span data-stu-id="78f56-108">Properties</span></span>
| <span data-ttu-id="78f56-109">属性</span><span class="sxs-lookup"><span data-stu-id="78f56-109">Property</span></span> | <span data-ttu-id="78f56-110">类型</span><span class="sxs-lookup"><span data-stu-id="78f56-110">Type</span></span> | <span data-ttu-id="78f56-111">说明</span><span class="sxs-lookup"><span data-stu-id="78f56-111">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="78f56-112">查询</span><span class="sxs-lookup"><span data-stu-id="78f56-112">query</span></span> | <span data-ttu-id="78f56-113">字符串</span><span class="sxs-lookup"><span data-stu-id="78f56-113">String</span></span> | <span data-ttu-id="78f56-114">用于指定审阅者的查询。</span><span class="sxs-lookup"><span data-stu-id="78f56-114">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="78f56-115">有关示例，请参阅表。</span><span class="sxs-lookup"><span data-stu-id="78f56-115">See table for examples.</span></span> |
| <span data-ttu-id="78f56-116">queryType</span><span class="sxs-lookup"><span data-stu-id="78f56-116">queryType</span></span> | <span data-ttu-id="78f56-117">字符串</span><span class="sxs-lookup"><span data-stu-id="78f56-117">String</span></span> | <span data-ttu-id="78f56-118">查询的类型。</span><span class="sxs-lookup"><span data-stu-id="78f56-118">The type of query.</span></span> <span data-ttu-id="78f56-119">示例包括 `MicrosoftGraph` `ARM` 和 。</span><span class="sxs-lookup"><span data-stu-id="78f56-119">Examples include `MicrosoftGraph` and `ARM`.</span></span> |
| <span data-ttu-id="78f56-120">queryRoot</span><span class="sxs-lookup"><span data-stu-id="78f56-120">queryRoot</span></span> | <span data-ttu-id="78f56-121">字符串</span><span class="sxs-lookup"><span data-stu-id="78f56-121">String</span></span> | <span data-ttu-id="78f56-122">在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。</span><span class="sxs-lookup"><span data-stu-id="78f56-122">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="78f56-123">此属性仅在指定了相对查询 (./manager) 是必需的。</span><span class="sxs-lookup"><span data-stu-id="78f56-123">This property is only required if a relative query (i.e., ./manager) is specified.</span></span> |

### <a name="supported-queries-for-accessreviewreviewerscope"></a><span data-ttu-id="78f56-124">AccessReviewReviewerScope 支持的查询</span><span class="sxs-lookup"><span data-stu-id="78f56-124">Supported queries for accessReviewReviewerScope</span></span>

|<span data-ttu-id="78f56-125">应用场景</span><span class="sxs-lookup"><span data-stu-id="78f56-125">Scenario</span></span>| <span data-ttu-id="78f56-126">查询</span><span class="sxs-lookup"><span data-stu-id="78f56-126">query</span></span> | <span data-ttu-id="78f56-127">queryType</span><span class="sxs-lookup"><span data-stu-id="78f56-127">queryType</span></span> | <span data-ttu-id="78f56-128">queryRoot</span><span class="sxs-lookup"><span data-stu-id="78f56-128">queryRoot</span></span> |
|--|--|--|--|
| <span data-ttu-id="78f56-129">作为审阅者的组所有者</span><span class="sxs-lookup"><span data-stu-id="78f56-129">Group owner as reviewer</span></span> | <span data-ttu-id="78f56-130">/groups/{group id}/owners</span><span class="sxs-lookup"><span data-stu-id="78f56-130">/groups/{group id}/owners</span></span> |<span data-ttu-id="78f56-131">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="78f56-131">MicrosoftGraph</span></span>||
| <span data-ttu-id="78f56-132">特定用户作为审阅者</span><span class="sxs-lookup"><span data-stu-id="78f56-132">Specific user as reviewer</span></span> | <span data-ttu-id="78f56-133">/users/{user id}</span><span class="sxs-lookup"><span data-stu-id="78f56-133">/users/{user id}</span></span> |<span data-ttu-id="78f56-134">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="78f56-134">MicrosoftGraph</span></span>||
| <span data-ttu-id="78f56-135">被审阅为审阅者的用户的经理</span><span class="sxs-lookup"><span data-stu-id="78f56-135">Manager of user being reviewed as reviewer</span></span> | <span data-ttu-id="78f56-136">./manager</span><span class="sxs-lookup"><span data-stu-id="78f56-136">./manager</span></span> | <span data-ttu-id="78f56-137">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="78f56-137">MicrosoftGraph</span></span> |<span data-ttu-id="78f56-138">决策</span><span class="sxs-lookup"><span data-stu-id="78f56-138">decisions</span></span>|

## <a name="relationships"></a><span data-ttu-id="78f56-139">关系</span><span class="sxs-lookup"><span data-stu-id="78f56-139">Relationships</span></span>
<span data-ttu-id="78f56-140">无。</span><span class="sxs-lookup"><span data-stu-id="78f56-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="78f56-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78f56-141">JSON representation</span></span>
<span data-ttu-id="78f56-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78f56-142">The following is a JSON representation of the resource.</span></span>
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
