---
title: accessReviewReviewerScope 资源类型
description: 表示将查看访问评审的团队。
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: edc25e19a51f787dd0799fbd9e6e6c2a1b45787e
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000839"
---
# <a name="accessreviewreviewerscope-resource-type"></a><span data-ttu-id="a760e-103">accessReviewReviewerScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="a760e-103">accessReviewReviewerScope resource type</span></span>

<span data-ttu-id="a760e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a760e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a760e-105">AccessReviewReviewerScope 定义了将审阅 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)实例的作者。</span><span class="sxs-lookup"><span data-stu-id="a760e-105">The accessReviewReviewerScope defines who will review instances of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="a760e-106">这表示为 OData 查询，该查询允许将审阅者指定为用户的静态列表 (即特定用户、组所有者、组成员) 或动态 (（即，每个用户被其经理) 审阅的情况）。</span><span class="sxs-lookup"><span data-stu-id="a760e-106">This is expressed as an OData query, which allows reviewers to be specified both as a static list of users (i.e., specific users, group owners, group members) or dynamically (i.e., the case where every user is reviewed by their manager).</span></span> <span data-ttu-id="a760e-107">若要创建一个自我审阅 (用户在其中查看自己的访问) ，请不要在创建 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) 的情况下提供审阅者。</span><span class="sxs-lookup"><span data-stu-id="a760e-107">To create a self-review (where users review their own access), do not provide reviewers on [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) creation.</span></span>


## <a name="properties"></a><span data-ttu-id="a760e-108">属性</span><span class="sxs-lookup"><span data-stu-id="a760e-108">Properties</span></span>
| <span data-ttu-id="a760e-109">属性</span><span class="sxs-lookup"><span data-stu-id="a760e-109">Property</span></span> | <span data-ttu-id="a760e-110">类型</span><span class="sxs-lookup"><span data-stu-id="a760e-110">Type</span></span> | <span data-ttu-id="a760e-111">说明</span><span class="sxs-lookup"><span data-stu-id="a760e-111">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="a760e-112">查询</span><span class="sxs-lookup"><span data-stu-id="a760e-112">query</span></span> | <span data-ttu-id="a760e-113">字符串</span><span class="sxs-lookup"><span data-stu-id="a760e-113">String</span></span> | <span data-ttu-id="a760e-114">指定将成为审阅者的查询。</span><span class="sxs-lookup"><span data-stu-id="a760e-114">The query specifying who will be the reviewer.</span></span> <span data-ttu-id="a760e-115">有关示例，请参阅 table。</span><span class="sxs-lookup"><span data-stu-id="a760e-115">See table for examples.</span></span> |
| <span data-ttu-id="a760e-116">queryType</span><span class="sxs-lookup"><span data-stu-id="a760e-116">queryType</span></span> | <span data-ttu-id="a760e-117">字符串</span><span class="sxs-lookup"><span data-stu-id="a760e-117">String</span></span> | <span data-ttu-id="a760e-118">查询的类型。</span><span class="sxs-lookup"><span data-stu-id="a760e-118">The type of query.</span></span> <span data-ttu-id="a760e-119">示例包括 `MicrosoftGraph` 和 `ARM` 。</span><span class="sxs-lookup"><span data-stu-id="a760e-119">Examples include `MicrosoftGraph` and `ARM`.</span></span> |
| <span data-ttu-id="a760e-120">queryRoot</span><span class="sxs-lookup"><span data-stu-id="a760e-120">queryRoot</span></span> | <span data-ttu-id="a760e-121">字符串</span><span class="sxs-lookup"><span data-stu-id="a760e-121">String</span></span> | <span data-ttu-id="a760e-122">在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。</span><span class="sxs-lookup"><span data-stu-id="a760e-122">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="a760e-123">仅当指定相对查询 (（即/manager) ）时，此属性才是必需的。</span><span class="sxs-lookup"><span data-stu-id="a760e-123">This property is only required if a relative query (i.e., ./manager) is specified.</span></span> |

### <a name="supported-queries-for-accessreviewreviewerscope"></a><span data-ttu-id="a760e-124">AccessReviewReviewerScope 支持的查询</span><span class="sxs-lookup"><span data-stu-id="a760e-124">Supported queries for accessReviewReviewerScope</span></span>

|<span data-ttu-id="a760e-125">应用场景</span><span class="sxs-lookup"><span data-stu-id="a760e-125">Scenario</span></span>| <span data-ttu-id="a760e-126">查询</span><span class="sxs-lookup"><span data-stu-id="a760e-126">query</span></span> | <span data-ttu-id="a760e-127">queryType</span><span class="sxs-lookup"><span data-stu-id="a760e-127">queryType</span></span> | <span data-ttu-id="a760e-128">queryRoot</span><span class="sxs-lookup"><span data-stu-id="a760e-128">queryRoot</span></span> |
|--|--|--|--|
| <span data-ttu-id="a760e-129">将所有者分组为审阅人</span><span class="sxs-lookup"><span data-stu-id="a760e-129">Group owner as reviewer</span></span> | <span data-ttu-id="a760e-130">/groups/{group id}/owners</span><span class="sxs-lookup"><span data-stu-id="a760e-130">/groups/{group id}/owners</span></span> |<span data-ttu-id="a760e-131">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="a760e-131">MicrosoftGraph</span></span>||
| <span data-ttu-id="a760e-132">作为审阅者的特定用户</span><span class="sxs-lookup"><span data-stu-id="a760e-132">Specific user as reviewer</span></span> | <span data-ttu-id="a760e-133">/users/{user id}</span><span class="sxs-lookup"><span data-stu-id="a760e-133">/users/{user id}</span></span> |<span data-ttu-id="a760e-134">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="a760e-134">MicrosoftGraph</span></span>||
| <span data-ttu-id="a760e-135">被审阅为审阅者的用户管理者</span><span class="sxs-lookup"><span data-stu-id="a760e-135">Manager of user being reviewed as reviewer</span></span> | <span data-ttu-id="a760e-136">./manager</span><span class="sxs-lookup"><span data-stu-id="a760e-136">./manager</span></span> | <span data-ttu-id="a760e-137">MicrosoftGraph</span><span class="sxs-lookup"><span data-stu-id="a760e-137">MicrosoftGraph</span></span> |<span data-ttu-id="a760e-138">针对</span><span class="sxs-lookup"><span data-stu-id="a760e-138">decisions</span></span>|

## <a name="relationships"></a><span data-ttu-id="a760e-139">关系</span><span class="sxs-lookup"><span data-stu-id="a760e-139">Relationships</span></span>
<span data-ttu-id="a760e-140">无。</span><span class="sxs-lookup"><span data-stu-id="a760e-140">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a760e-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a760e-141">JSON representation</span></span>
<span data-ttu-id="a760e-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a760e-142">The following is a JSON representation of the resource.</span></span>
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
