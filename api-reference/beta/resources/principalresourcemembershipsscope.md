---
title: principalResourceMembershipsScope 资源类型
description: 允许选择范围查看所选主体对选定资源的访问权限。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 2ac3dd53223b9260c3f51c3c872d36b044e698d5
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469742"
---
# <a name="principalresourcemembershipsscope-resource-type"></a><span data-ttu-id="88234-103">principalResourceMembershipsScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="88234-103">principalResourceMembershipsScope resource type</span></span>

<span data-ttu-id="88234-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88234-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

<span data-ttu-id="88234-105">principalResourceMembershipsScope 是 [accessReviewScope](accessreviewscope.md) 的一种类型，它允许您选择主体作用域的集合和资源作用域的集合，并查看所选主体对选定资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="88234-105">The principalResourceMembershipsScope is a type of [accessReviewScope](accessreviewscope.md) which allows you to select a collection of principal scopes and a collection of resource scopes and review access of selected principals to selected resources.</span></span> <span data-ttu-id="88234-106">请参阅受支持的查询以查看可以选择哪些查询。</span><span class="sxs-lookup"><span data-stu-id="88234-106">See the supported queries to see what can be selected.</span></span> <span data-ttu-id="88234-107">它用作 `scope` [accessReviewScheduleDefinition 的属性](accessreviewscheduledefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="88234-107">It is used as the `scope` property of an [accessReviewScheduleDefinition](accessreviewscheduledefinition.md).</span></span>

<span data-ttu-id="88234-108">继承自 [accessReviewScope](../resources/accessreviewscope.md)。</span><span class="sxs-lookup"><span data-stu-id="88234-108">Inherits from [accessReviewScope](../resources/accessreviewscope.md).</span></span>

## <a name="properties"></a><span data-ttu-id="88234-109">属性</span><span class="sxs-lookup"><span data-stu-id="88234-109">Properties</span></span>
|<span data-ttu-id="88234-110">属性</span><span class="sxs-lookup"><span data-stu-id="88234-110">Property</span></span>|<span data-ttu-id="88234-111">类型</span><span class="sxs-lookup"><span data-stu-id="88234-111">Type</span></span>|<span data-ttu-id="88234-112">说明</span><span class="sxs-lookup"><span data-stu-id="88234-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88234-113">principalScopes</span><span class="sxs-lookup"><span data-stu-id="88234-113">principalScopes</span></span>|<span data-ttu-id="88234-114">[accessReviewScope](../resources/accessreviewscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88234-114">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="88234-115">定义要包含在访问评审中的主体范围。</span><span class="sxs-lookup"><span data-stu-id="88234-115">Defines the scopes of the principals to be included in an access review.</span></span>|
|<span data-ttu-id="88234-116">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="88234-116">resourceScopes</span></span>|<span data-ttu-id="88234-117">[accessReviewScope](../resources/accessreviewscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="88234-117">[accessReviewScope](../resources/accessreviewscope.md) collection</span></span>|<span data-ttu-id="88234-118">定义将检查其访问权限的资源的范围。</span><span class="sxs-lookup"><span data-stu-id="88234-118">Defines the scopes of the resources for which access will be reviewed.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88234-119">关系</span><span class="sxs-lookup"><span data-stu-id="88234-119">Relationships</span></span>
<span data-ttu-id="88234-120">无。</span><span class="sxs-lookup"><span data-stu-id="88234-120">None.</span></span>

### <a name="supported-queries-for-resourcescope"></a><span data-ttu-id="88234-121">resourceScope 支持的查询</span><span class="sxs-lookup"><span data-stu-id="88234-121">Supported queries for resourceScope</span></span>
<span data-ttu-id="88234-122">支持将查询作为 `resourceScope` 属性。</span><span class="sxs-lookup"><span data-stu-id="88234-122">The queries are supported as the `resourceScope` property.</span></span> <span data-ttu-id="88234-123">它们确定要检查的资源访问权限集。</span><span class="sxs-lookup"><span data-stu-id="88234-123">They determine the set of resources access is being reviewed to.</span></span> 

|<span data-ttu-id="88234-124">方案</span><span class="sxs-lookup"><span data-stu-id="88234-124">Scenario</span></span>| <span data-ttu-id="88234-125">resourceScope 查询</span><span class="sxs-lookup"><span data-stu-id="88234-125">resourceScope Query</span></span> | 
|--|--|
| <span data-ttu-id="88234-126">查看对服务主体的 principalScopes 的访问</span><span class="sxs-lookup"><span data-stu-id="88234-126">Reviewing access of principalScopes to a service principal</span></span> | <span data-ttu-id="88234-127">/servicePrincipals/{service principal ID}</span><span class="sxs-lookup"><span data-stu-id="88234-127">/servicePrincipals/{service principal ID}</span></span> |
| <span data-ttu-id="88234-128">查看对 Azure AD 目录角色的 principalScopes 的访问权限</span><span class="sxs-lookup"><span data-stu-id="88234-128">Reviewing access of principalScopes to an Azure AD directory role</span></span> | <span data-ttu-id="88234-129">/roleManagement/directory/roleDefinitions/{role ID}</span><span class="sxs-lookup"><span data-stu-id="88234-129">/roleManagement/directory/roleDefinitions/{role ID}</span></span> |
| <span data-ttu-id="88234-130">查看所有 Azure AD 目录角色对 principalScopes 的访问权限</span><span class="sxs-lookup"><span data-stu-id="88234-130">Reviewing access of principalScopes to all Azure AD directory roles</span></span> | <span data-ttu-id="88234-131">/roleManagement/directory/roleDefinitions</span><span class="sxs-lookup"><span data-stu-id="88234-131">/roleManagement/directory/roleDefinitions</span></span> |

### <a name="supported-queries-for-principalscope"></a><span data-ttu-id="88234-132">principalScope 支持的查询</span><span class="sxs-lookup"><span data-stu-id="88234-132">Supported queries for principalScope</span></span>
<span data-ttu-id="88234-133">支持将查询作为 `principalScope` 属性。</span><span class="sxs-lookup"><span data-stu-id="88234-133">The queries are supported as the `principalScope` property.</span></span> <span data-ttu-id="88234-134">它们确定将检查其对关联 resourceScope 的访问权的主体集。</span><span class="sxs-lookup"><span data-stu-id="88234-134">They determine the set of principals whose access to the associated resourceScope will be reviewed.</span></span> <span data-ttu-id="88234-135">关联的 principalScope 类型列出了接受为 principalScope 的 odata 查询类型。</span><span class="sxs-lookup"><span data-stu-id="88234-135">The associated principalScope Type lists the odata query types accepted as the principalScope.</span></span>

|<span data-ttu-id="88234-136">方案</span><span class="sxs-lookup"><span data-stu-id="88234-136">Scenario</span></span>| <span data-ttu-id="88234-137">principalScope 查询</span><span class="sxs-lookup"><span data-stu-id="88234-137">principalScope Query</span></span> | <span data-ttu-id="88234-138">OData 查询类型</span><span class="sxs-lookup"><span data-stu-id="88234-138">OData Query Type</span></span> | <span data-ttu-id="88234-139">其他注释</span><span class="sxs-lookup"><span data-stu-id="88234-139">Additional Comments</span></span> |
|--|--|-- | --|
| <span data-ttu-id="88234-140">查看所有用户对 resourceScope 的访问权限</span><span class="sxs-lookup"><span data-stu-id="88234-140">Review access of all users to the resourceScope</span></span> | <span data-ttu-id="88234-141">/users</span><span class="sxs-lookup"><span data-stu-id="88234-141">/users</span></span> |[<span data-ttu-id="88234-142">accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="88234-142">accessReviewQueryScope</span></span>](accessreviewqueryscope.md)||
| <span data-ttu-id="88234-143">查看来宾用户对 resourceScope 的访问权限</span><span class="sxs-lookup"><span data-stu-id="88234-143">Review access of  guest users to the resourceScope</span></span> | <span data-ttu-id="88234-144">/users？$filter= (userType eq 'Guest') </span><span class="sxs-lookup"><span data-stu-id="88234-144">/users?$filter=(userType eq 'Guest')</span></span> |[<span data-ttu-id="88234-145">accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="88234-145">accessReviewQueryScope</span></span>](accessreviewqueryscope.md)||
| <span data-ttu-id="88234-146">查看所有非活动用户对 resourceScope 的访问权限</span><span class="sxs-lookup"><span data-stu-id="88234-146">Review access of all inactive users to the resourceScope</span></span> | <span data-ttu-id="88234-147">/users</span><span class="sxs-lookup"><span data-stu-id="88234-147">/users</span></span> |[<span data-ttu-id="88234-148">accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="88234-148">accessReviewInactiveUsersQueryScope</span></span>](accessreviewinactiveusersqueryscope.md)| <span data-ttu-id="88234-149">必须包含 `instanceDuration` 属性</span><span class="sxs-lookup"><span data-stu-id="88234-149">Must include `instanceDuration` property</span></span>|
| <span data-ttu-id="88234-150">查看对 resourceScope 的来宾非活动用户的访问权限</span><span class="sxs-lookup"><span data-stu-id="88234-150">Review access of guest inactive users to the resourceScope</span></span> | <span data-ttu-id="88234-151">/users？$filter= (userType eq 'Guest') </span><span class="sxs-lookup"><span data-stu-id="88234-151">/users?$filter=(userType eq 'Guest')</span></span> |[<span data-ttu-id="88234-152">accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="88234-152">accessReviewInactiveUsersQueryScope</span></span>](accessreviewinactiveusersqueryscope.md)| <span data-ttu-id="88234-153">必须包含 `instanceDuration` 属性</span><span class="sxs-lookup"><span data-stu-id="88234-153">Must include `instanceDuration` property</span></span>|




## <a name="json-representation"></a><span data-ttu-id="88234-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="88234-154">JSON representation</span></span>
<span data-ttu-id="88234-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88234-155">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.principalResourceMembershipsScope"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
  "principalScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ],
  "resourceScopes": [
    {
      "@odata.type": "microsoft.graph.accessReviewScope"
    }
  ]
}
```
