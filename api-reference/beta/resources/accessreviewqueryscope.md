---
title: accessReviewQueryScope 资源类型
description: 定义在访问评审中将审阅哪些项。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 976a856755b6bb638719bec6006c3d8d0587c42a
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469747"
---
# <a name="accessreviewqueryscope-resource-type"></a><span data-ttu-id="cba78-103">accessReviewQueryScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="cba78-103">accessReviewQueryScope resource type</span></span>

<span data-ttu-id="cba78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cba78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="cba78-105">accessReviewQueryScope 对象定义将在 [accessReview 中查看哪些项](../resources/accessreviewsv2-root.md)。</span><span class="sxs-lookup"><span data-stu-id="cba78-105">An accessReviewQueryScope object defines what will be reviewed in an [accessReview](../resources/accessreviewsv2-root.md).</span></span> <span data-ttu-id="cba78-106">请参阅支持的查询以查看选择选项。</span><span class="sxs-lookup"><span data-stu-id="cba78-106">See the supported queries to see the selection options.</span></span> <span data-ttu-id="cba78-107">若要将访问评审的范围确定为非活动用户，请参阅 [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md)。</span><span class="sxs-lookup"><span data-stu-id="cba78-107">To scope an access review to inactive users, see [accessReviewInactiveUserQueryScope](../resources/accessreviewinactiveusersqueryscope.md).</span></span> 

<span data-ttu-id="cba78-108">继承自 [accessReviewScope](../resources/accessreviewscope.md)。</span><span class="sxs-lookup"><span data-stu-id="cba78-108">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cba78-109">属性</span><span class="sxs-lookup"><span data-stu-id="cba78-109">Properties</span></span>
|<span data-ttu-id="cba78-110">属性</span><span class="sxs-lookup"><span data-stu-id="cba78-110">Property</span></span>|<span data-ttu-id="cba78-111">类型</span><span class="sxs-lookup"><span data-stu-id="cba78-111">Type</span></span>|<span data-ttu-id="cba78-112">说明</span><span class="sxs-lookup"><span data-stu-id="cba78-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cba78-113">查询</span><span class="sxs-lookup"><span data-stu-id="cba78-113">query</span></span>|<span data-ttu-id="cba78-114">String</span><span class="sxs-lookup"><span data-stu-id="cba78-114">String</span></span>|<span data-ttu-id="cba78-115">表示将在访问评审中审阅哪些内容的查询。</span><span class="sxs-lookup"><span data-stu-id="cba78-115">The query representing what will be reviewed in an access review.</span></span> <span data-ttu-id="cba78-116">例如 ，/groups/{id}/members？$filter=...</span><span class="sxs-lookup"><span data-stu-id="cba78-116">Examples of this include /groups/{id}/members?$filter=…</span></span>|
|<span data-ttu-id="cba78-117">queryRoot</span><span class="sxs-lookup"><span data-stu-id="cba78-117">queryRoot</span></span>|<span data-ttu-id="cba78-118">String</span><span class="sxs-lookup"><span data-stu-id="cba78-118">String</span></span>|<span data-ttu-id="cba78-119">在需要动态指定审阅者的情况下，此属性用于指示查询的相对源。</span><span class="sxs-lookup"><span data-stu-id="cba78-119">In the scenario where reviewers need to be specified dynamically, this property is used to indicate the relative source of the query.</span></span> <span data-ttu-id="cba78-120">此属性仅在指定了相对查询时是必需的。</span><span class="sxs-lookup"><span data-stu-id="cba78-120">This property is only required if a relative query is specified.</span></span> <span data-ttu-id="cba78-121">例如，`./manager`。</span><span class="sxs-lookup"><span data-stu-id="cba78-121">For example, `./manager`.</span></span>|
|<span data-ttu-id="cba78-122">queryType</span><span class="sxs-lookup"><span data-stu-id="cba78-122">queryType</span></span>|<span data-ttu-id="cba78-123">String</span><span class="sxs-lookup"><span data-stu-id="cba78-123">String</span></span>|<span data-ttu-id="cba78-124">指示查询的类型。</span><span class="sxs-lookup"><span data-stu-id="cba78-124">Indicates the type of query.</span></span> <span data-ttu-id="cba78-125">类型包括 MicrosoftGraph 和 ARM。</span><span class="sxs-lookup"><span data-stu-id="cba78-125">Types include MicrosoftGraph and ARM.</span></span>|

### <a name="supported-queries-for-accessreviewqueryscope-as-scope"></a><span data-ttu-id="cba78-126">accessReviewQueryScope 作为范围的受支持的查询</span><span class="sxs-lookup"><span data-stu-id="cba78-126">Supported queries for accessReviewQueryScope as scope</span></span>
<span data-ttu-id="cba78-127">这些查询作为 `scope` [accessReviewScheduleDefinition 中的 属性受到支持](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cba78-127">The queries are supported as the `scope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="cba78-128">方案</span><span class="sxs-lookup"><span data-stu-id="cba78-128">Scenario</span></span>| <span data-ttu-id="cba78-129">查询</span><span class="sxs-lookup"><span data-stu-id="cba78-129">Query</span></span> | <span data-ttu-id="cba78-130">其他注释</span><span class="sxs-lookup"><span data-stu-id="cba78-130">Additional Comments</span></span> |
|--|--|-- |
| <span data-ttu-id="cba78-131">查看分配给组的所有用户</span><span class="sxs-lookup"><span data-stu-id="cba78-131">Review of all users assigned to a group</span></span> | <span data-ttu-id="cba78-132">/groups/{group id}/transitiveMembers</span><span class="sxs-lookup"><span data-stu-id="cba78-132">/groups/{group id}/transitiveMembers</span></span> ||
| <span data-ttu-id="cba78-133">查看分配给组的来宾用户</span><span class="sxs-lookup"><span data-stu-id="cba78-133">Review of guest users assigned to a group</span></span> | <span data-ttu-id="cba78-134">/groups/{group id}/microsoft.graph.user/？$count=true&$filter= (userType eq 'Guest') </span><span class="sxs-lookup"><span data-stu-id="cba78-134">/groups/{group id}/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> ||
| <span data-ttu-id="cba78-135">查看分配给所有 Microsoft 365 组的来宾用户</span><span class="sxs-lookup"><span data-stu-id="cba78-135">Review of guest users assigned to all Microsoft 365 groups</span></span> | <span data-ttu-id="cba78-136">./members/microsoft.graph.user/？$count=true&$filter= (userType eq 'Guest') </span><span class="sxs-lookup"><span data-stu-id="cba78-136">./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')</span></span> | <span data-ttu-id="cba78-137">请注意，相应的 instanceEnumerationScope 还应传递到 accessReviewScheduleDefinition。</span><span class="sxs-lookup"><span data-stu-id="cba78-137">Note that the corresponding instanceEnumerationScope should also be passed in to the accessReviewScheduleDefinition.</span></span> <span data-ttu-id="cba78-138">有关 instanceEnumerationScope 查询，请参阅下表。</span><span class="sxs-lookup"><span data-stu-id="cba78-138">See table below for instanceEnumerationScope query.</span></span> |
| <span data-ttu-id="cba78-139">权利管理访问包分配评审</span><span class="sxs-lookup"><span data-stu-id="cba78-139">Entitlement Management Access Package Assignment Reviews</span></span> | <span data-ttu-id="cba78-140">/identityGovernance/entitlementManagement/accessPackageAssignments？$filter= (accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}') </span><span class="sxs-lookup"><span data-stu-id="cba78-140">/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')</span></span>| <span data-ttu-id="cba78-141">请注意，Access Package Assignment Reviews 仅支持 READ</span><span class="sxs-lookup"><span data-stu-id="cba78-141">Note that only READ is supported for Access Package Assignment Reviews</span></span>|
| <span data-ttu-id="cba78-142">查看分配给特权角色的服务主体</span><span class="sxs-lookup"><span data-stu-id="cba78-142">Review of Service Principals assigned to privileged roles</span></span> | <span data-ttu-id="cba78-143">/beta/roleManagement/directory/roleAssignmentScheduleInstances？$expand=principal&$filter= (isof (principal，'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}') </span><span class="sxs-lookup"><span data-stu-id="cba78-143">/beta/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')</span></span> | |

### <a name="supported-queries-for-instanceenumerationscope"></a><span data-ttu-id="cba78-144">instanceEnumerationScope 支持的查询</span><span class="sxs-lookup"><span data-stu-id="cba78-144">Supported queries for instanceEnumerationScope</span></span> 
<span data-ttu-id="cba78-145">这些查询作为 `instanceEnumerationScope` [accessReviewScheduleDefinition 中的 属性受到支持](accessreviewscheduledefinition.md)</span><span class="sxs-lookup"><span data-stu-id="cba78-145">The queries are supported as the `instanceEnumerationScope` property in an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md)</span></span>

|<span data-ttu-id="cba78-146">方案</span><span class="sxs-lookup"><span data-stu-id="cba78-146">Scenario</span></span>| <span data-ttu-id="cba78-147">查询</span><span class="sxs-lookup"><span data-stu-id="cba78-147">Query</span></span> | <span data-ttu-id="cba78-148">其他注释</span><span class="sxs-lookup"><span data-stu-id="cba78-148">Additional Comments</span></span> |
|--|--|--|
|  <span data-ttu-id="cba78-149">查看分配给所有 Microsoft 365 组的来宾用户</span><span class="sxs-lookup"><span data-stu-id="cba78-149">Review of guest users assigned to all Microsoft 365 groups</span></span>| <span data-ttu-id="cba78-150">/v1.0/groups？ \$filter= (groupTypes/any (c：c+eq+'Unified') ) &$count=true</span><span class="sxs-lookup"><span data-stu-id="cba78-150">/v1.0/groups?\$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true</span></span> | <span data-ttu-id="cba78-151">请注意，相应的作用域也应随以下项一起传入</span><span class="sxs-lookup"><span data-stu-id="cba78-151">Note that the corresponding scope should also be passed in along with this</span></span>|
| <span data-ttu-id="cba78-152">查看分配给所有团队的来宾用户</span><span class="sxs-lookup"><span data-stu-id="cba78-152">Review of guest users assigned to all teams</span></span> | <span data-ttu-id="cba78-153">/v1.0/groups？ \$filter= (groupTypes/any (c：c+eq+'Unified') and resourceProvisioningOptions/Any (x：x eq 'Team') ) &$count=true</span><span class="sxs-lookup"><span data-stu-id="cba78-153">/v1.0/groups?\$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team'))&$count=true</span></span> | <span data-ttu-id="cba78-154">请注意，相应的作用域也应随以下项一起传入</span><span class="sxs-lookup"><span data-stu-id="cba78-154">Note that the corresponding scope should also be passed in along with this</span></span>|

## <a name="relationships"></a><span data-ttu-id="cba78-155">关系</span><span class="sxs-lookup"><span data-stu-id="cba78-155">Relationships</span></span>
<span data-ttu-id="cba78-156">无。</span><span class="sxs-lookup"><span data-stu-id="cba78-156">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cba78-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cba78-157">JSON representation</span></span>
<span data-ttu-id="cba78-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cba78-158">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.accessReviewQueryScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewQueryScope",
  "query": "String",
  "queryType": "String",
  "queryRoot": "String"
}
```
