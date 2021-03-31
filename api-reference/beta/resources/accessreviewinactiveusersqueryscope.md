---
title: accessReviewInactiveUsersQueryScope 资源类型
description: 一种 accessReviewQueryScope 类型，只允许在访问评审范围内选择非活动用户。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 51fc61ce186b0346bc065ddc5dfea40158758223
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469748"
---
# <a name="accessreviewinactiveusersqueryscope-resource-type"></a><span data-ttu-id="24128-103">accessReviewInactiveUsersQueryScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="24128-103">accessReviewInactiveUsersQueryScope resource type</span></span>

<span data-ttu-id="24128-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24128-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="24128-105">一种 [accessReviewQueryScope](../resources/accessreviewqueryscope.md) 类型，只允许在访问评审范围内选择非活动用户。</span><span class="sxs-lookup"><span data-stu-id="24128-105">A type of [accessReviewQueryScope](../resources/accessreviewqueryscope.md) that allows only inactive users to be selected in the scope of an access review.</span></span>

<span data-ttu-id="24128-106">继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="24128-106">Inherits from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="24128-107">属性</span><span class="sxs-lookup"><span data-stu-id="24128-107">Properties</span></span>
|<span data-ttu-id="24128-108">属性</span><span class="sxs-lookup"><span data-stu-id="24128-108">Property</span></span>|<span data-ttu-id="24128-109">类型</span><span class="sxs-lookup"><span data-stu-id="24128-109">Type</span></span>|<span data-ttu-id="24128-110">说明</span><span class="sxs-lookup"><span data-stu-id="24128-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24128-111">inactiveDuration</span><span class="sxs-lookup"><span data-stu-id="24128-111">inactiveDuration</span></span>|<span data-ttu-id="24128-112">持续时间</span><span class="sxs-lookup"><span data-stu-id="24128-112">Duration</span></span>|<span data-ttu-id="24128-113">定义不活动持续时间的长度。</span><span class="sxs-lookup"><span data-stu-id="24128-113">Defines the length of the duration period of inactivity.</span></span> <span data-ttu-id="24128-114">不活动基于用户的上次登录日期。</span><span class="sxs-lookup"><span data-stu-id="24128-114">Inactivity is based on the last sign in date of the user.</span></span>|
|<span data-ttu-id="24128-115">查询</span><span class="sxs-lookup"><span data-stu-id="24128-115">query</span></span>|<span data-ttu-id="24128-116">String</span><span class="sxs-lookup"><span data-stu-id="24128-116">String</span></span>|<span data-ttu-id="24128-117">继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="24128-117">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="24128-118">queryRoot</span><span class="sxs-lookup"><span data-stu-id="24128-118">queryRoot</span></span>|<span data-ttu-id="24128-119">String</span><span class="sxs-lookup"><span data-stu-id="24128-119">String</span></span>|<span data-ttu-id="24128-120">继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="24128-120">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|
|<span data-ttu-id="24128-121">queryType</span><span class="sxs-lookup"><span data-stu-id="24128-121">queryType</span></span>|<span data-ttu-id="24128-122">String</span><span class="sxs-lookup"><span data-stu-id="24128-122">String</span></span>|<span data-ttu-id="24128-123">继承自 [accessReviewQueryScope](../resources/accessreviewqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="24128-123">Inherited from [accessReviewQueryScope](../resources/accessreviewqueryscope.md).</span></span>|

### <a name="supported-queries-for-accessreviewinactiveuserqueryscope-as-scope"></a><span data-ttu-id="24128-124">accessReviewInactiveUserQueryScope 作为范围的受支持的查询</span><span class="sxs-lookup"><span data-stu-id="24128-124">Supported queries for accessReviewInactiveUserQueryScope as scope</span></span>
<span data-ttu-id="24128-125">[accessReviewScope](../resources/accessreviewscope.md)上支持的相同查询在 accessReviewInactiveUserQueryScope 上也受支持。</span><span class="sxs-lookup"><span data-stu-id="24128-125">The same queries supported on [accessReviewScope](../resources/accessreviewscope.md) are also supported on accessReviewInactiveUserQueryScope.</span></span> <span data-ttu-id="24128-126">以下是查询。</span><span class="sxs-lookup"><span data-stu-id="24128-126">The following are the queries.</span></span> <span data-ttu-id="24128-127">它们作为 `scope` [accessReviewScheduleDefinition 中的 属性受到支持](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="24128-127">They are supported as the `scope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span>

|<span data-ttu-id="24128-128">方案</span><span class="sxs-lookup"><span data-stu-id="24128-128">Scenario</span></span>| <span data-ttu-id="24128-129">查询</span><span class="sxs-lookup"><span data-stu-id="24128-129">Query</span></span> |
|--|--|
| <span data-ttu-id="24128-130">查看分配给组的所有非活动来宾用户</span><span class="sxs-lookup"><span data-stu-id="24128-130">Review all inactive guest users assigned to a group</span></span> | <span data-ttu-id="24128-131">/groups/{group ID}/transitiveMembers/microsoft.graph.user/？ \$count=true&$filter= (userType eq 'Guest') </span><span class="sxs-lookup"><span data-stu-id="24128-131">/groups/{group ID}/transitiveMembers/microsoft.graph.user/?\$count=true&$filter=(userType eq 'Guest')</span></span> |
| <span data-ttu-id="24128-132">查看分配给组的所有非活动用户</span><span class="sxs-lookup"><span data-stu-id="24128-132">Review all inactive users assigned to a group</span></span> | <span data-ttu-id="24128-133">/groups/{group ID}/transitiveMembers</span><span class="sxs-lookup"><span data-stu-id="24128-133">/groups/{group ID}/transitiveMembers</span></span> |
| <span data-ttu-id="24128-134">查看分配给所有组的所有非活动来宾用户</span><span class="sxs-lookup"><span data-stu-id="24128-134">Review all inactive guest users assigned to all groups</span></span> | <span data-ttu-id="24128-135">./members/microsoft.graph.user/？ \$count=true&$filter= (userType eq 'Guest') </span><span class="sxs-lookup"><span data-stu-id="24128-135">./members/microsoft.graph.user/?\$count=true&$filter=(userType eq 'Guest')</span></span> |


## <a name="relationships"></a><span data-ttu-id="24128-136">关系</span><span class="sxs-lookup"><span data-stu-id="24128-136">Relationships</span></span>
<span data-ttu-id="24128-137">无。</span><span class="sxs-lookup"><span data-stu-id="24128-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="24128-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24128-138">JSON representation</span></span>
<span data-ttu-id="24128-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24128-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewInactiveUsersQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String",
  "inactiveDuration": "String (duration)"
}
```
