---
title: accessReviewScope 资源类型
description: '在 "Azure AD 访问评论" 功能中， `accessReviewScope` 表示将在访问评审中审阅的实体。  '
author: isabelleatmsft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: af5a9bde0763f8aea9e28dc74832586c9e0d2e82
ms.sourcegitcommit: bbb617f16b40947769b262e6e85f0dea8a18ed3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2020
ms.locfileid: "49000831"
---
# <a name="accessreviewscope-resource-type"></a><span data-ttu-id="69cdb-103">accessReviewScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="69cdb-103">accessReviewScope resource type</span></span>

<span data-ttu-id="69cdb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69cdb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69cdb-105">**AccessReviewScope** 定义将在 [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)中审阅的实体。</span><span class="sxs-lookup"><span data-stu-id="69cdb-105">The **accessReviewScope** defines what entities will be reviewed in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span> <span data-ttu-id="69cdb-106">这表示为 odata 查询。</span><span class="sxs-lookup"><span data-stu-id="69cdb-106">This is expressed as an odata query.</span></span> <span data-ttu-id="69cdb-107">此外，还必须表示查询类型，以便可以支持在 MicrosoftGraph 之外查看实体（如 ARM）的方案。</span><span class="sxs-lookup"><span data-stu-id="69cdb-107">The query type must also be expressed so that scenarios can be supported to review entities outside of MicrosoftGraph, such as ARM.</span></span>

## <a name="properties"></a><span data-ttu-id="69cdb-108">属性</span><span class="sxs-lookup"><span data-stu-id="69cdb-108">Properties</span></span>
| <span data-ttu-id="69cdb-109">属性</span><span class="sxs-lookup"><span data-stu-id="69cdb-109">Property</span></span>   | <span data-ttu-id="69cdb-110">类型</span><span class="sxs-lookup"><span data-stu-id="69cdb-110">Type</span></span>  | <span data-ttu-id="69cdb-111">说明</span><span class="sxs-lookup"><span data-stu-id="69cdb-111">Description</span></span> |
| :-------------------------| :---------- | :---------- |
| <span data-ttu-id="69cdb-112">查询</span><span class="sxs-lookup"><span data-stu-id="69cdb-112">query</span></span> |<span data-ttu-id="69cdb-113">字符串</span><span class="sxs-lookup"><span data-stu-id="69cdb-113">String</span></span>  | <span data-ttu-id="69cdb-114">指定将评审的内容的查询。</span><span class="sxs-lookup"><span data-stu-id="69cdb-114">The query specifying what will be reviewed.</span></span> <span data-ttu-id="69cdb-115">有关示例，请参阅 table。</span><span class="sxs-lookup"><span data-stu-id="69cdb-115">See table for examples.</span></span> |
|<span data-ttu-id="69cdb-116">queryType</span><span class="sxs-lookup"><span data-stu-id="69cdb-116">queryType</span></span>  |<span data-ttu-id="69cdb-117">字符串</span><span class="sxs-lookup"><span data-stu-id="69cdb-117">String</span></span> | <span data-ttu-id="69cdb-118">查询的类型。</span><span class="sxs-lookup"><span data-stu-id="69cdb-118">The type of query.</span></span> <span data-ttu-id="69cdb-119">示例包括 MicrosoftGraph 和 ARM。</span><span class="sxs-lookup"><span data-stu-id="69cdb-119">Examples include MicrosoftGraph and ARM.</span></span> |

### <a name="supported-queries-for-accessreviewscope-as-scope"></a><span data-ttu-id="69cdb-120">支持的 accessReviewScope 作为范围的查询</span><span class="sxs-lookup"><span data-stu-id="69cdb-120">Supported queries for accessReviewScope as scope</span></span>
<span data-ttu-id="69cdb-121">以下是支持作为 `scope` [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)中的属性的查询。</span><span class="sxs-lookup"><span data-stu-id="69cdb-121">The following are queries supported as the `scope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="69cdb-122">应用场景</span><span class="sxs-lookup"><span data-stu-id="69cdb-122">Scenario</span></span>| <span data-ttu-id="69cdb-123">查询</span><span class="sxs-lookup"><span data-stu-id="69cdb-123">Query</span></span> | <span data-ttu-id="69cdb-124">其他注释</span><span class="sxs-lookup"><span data-stu-id="69cdb-124">Additional Comments</span></span> |
|--|--|-- |
| <span data-ttu-id="69cdb-125">查看分配给组的所有用户</span><span class="sxs-lookup"><span data-stu-id="69cdb-125">Review of all users assigned to a group</span></span> | <span data-ttu-id="69cdb-126">/groups/{group id}/transitiveMembers</span><span class="sxs-lookup"><span data-stu-id="69cdb-126">/groups/{group id}/transitiveMembers</span></span> ||
| <span data-ttu-id="69cdb-127">审阅分配给组的来宾用户</span><span class="sxs-lookup"><span data-stu-id="69cdb-127">Review of guest users assigned to a group</span></span> | <span data-ttu-id="69cdb-128">/groups/{group id}/microsoft.graph.user/？ $count = true&$filter = (userType eq ' Guest ' ) </span><span class="sxs-lookup"><span data-stu-id="69cdb-128">/groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> ||
| <span data-ttu-id="69cdb-129">查看分配给所有组的来宾用户</span><span class="sxs-lookup"><span data-stu-id="69cdb-129">Review of guest users assigned to all groups</span></span> | <span data-ttu-id="69cdb-130">./members/microsoft.graph.user/？ $count = true&$filter = (userType eq ' Guest ' ) </span><span class="sxs-lookup"><span data-stu-id="69cdb-130">./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> | <span data-ttu-id="69cdb-131">请注意，相应的 instanceEnumerationScope 也应传递给 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="69cdb-131">Note that the corresponding instanceEnumerationScope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="69cdb-132">有关 instanceEnumerationScope 查询，请参阅下表。</span><span class="sxs-lookup"><span data-stu-id="69cdb-132">See table below for instanceEnumerationScope query.</span></span> |
| <span data-ttu-id="69cdb-133">权利管理访问包 Assigment 评论</span><span class="sxs-lookup"><span data-stu-id="69cdb-133">Entitlement Management Access Package Assigment Reviews</span></span> | <span data-ttu-id="69cdb-134">$filter/identityGovernance/entitlementManagement/accessPackageAssignments = (accessPackageId eq ' {package id} ' 和 assignmentPolicyId eq ' {id} ' ) </span><span class="sxs-lookup"><span data-stu-id="69cdb-134">/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')</span></span>| <span data-ttu-id="69cdb-135">请注意，访问包分配审查仅支持读取</span><span class="sxs-lookup"><span data-stu-id="69cdb-135">Note that only READ is supported for Access Package Assignment Reviews</span></span>|

### <a name="supported-queries-for-accessreviewscope-as-instanceenumerationscope"></a><span data-ttu-id="69cdb-136">支持的 accessReviewScope 查询为 instanceEnumerationScope</span><span class="sxs-lookup"><span data-stu-id="69cdb-136">Supported queries for accessReviewScope as instanceEnumerationScope</span></span>
<span data-ttu-id="69cdb-137">以下是支持作为 `instanceEnumerationScope` [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)中的属性的查询。</span><span class="sxs-lookup"><span data-stu-id="69cdb-137">The following are queries supported as the `instanceEnumerationScope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="69cdb-138">应用场景</span><span class="sxs-lookup"><span data-stu-id="69cdb-138">Scenario</span></span>| <span data-ttu-id="69cdb-139">查询</span><span class="sxs-lookup"><span data-stu-id="69cdb-139">Query</span></span> | <span data-ttu-id="69cdb-140">其他注释</span><span class="sxs-lookup"><span data-stu-id="69cdb-140">Additional Comments</span></span> |
|--|--|--|
| <span data-ttu-id="69cdb-141">查看分配给所有组的来宾用户，但不包括指定的组</span><span class="sxs-lookup"><span data-stu-id="69cdb-141">Review of guest users assigned to all groups, excluding specified groups</span></span> | <span data-ttu-id="69cdb-142">$filter/groups = (groupTypes/any (c:c + eq + ' 统一 ' ) and id ne ' {group id} ' and id ne ' {group id} ' 和 id ne ' {group id} ' ) # B0 $count = true</span><span class="sxs-lookup"><span data-stu-id="69cdb-142">/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and id ne '{group id}' and id ne '{group id}' and id ne '{group id}')&$count=true</span></span> | <span data-ttu-id="69cdb-143">请注意，相应的作用域也应传递给 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="69cdb-143">Note that the corresponding scope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="69cdb-144">有关范围查询，请参阅上面的作用域属性表中的 "复查分配给所有组的来宾用户"。</span><span class="sxs-lookup"><span data-stu-id="69cdb-144">See "Review of guest users assigned to all groups" in scope property table above for the scope query.</span></span> |

## <a name="relationships"></a><span data-ttu-id="69cdb-145">关系</span><span class="sxs-lookup"><span data-stu-id="69cdb-145">Relationships</span></span>
<span data-ttu-id="69cdb-146">无。</span><span class="sxs-lookup"><span data-stu-id="69cdb-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="69cdb-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69cdb-147">JSON representation</span></span>
<span data-ttu-id="69cdb-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69cdb-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewScope",
  "query": "String",
  "queryType": "String"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "accessReviewScope resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
