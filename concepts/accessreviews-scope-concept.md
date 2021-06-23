---
title: 使用 Microsoft Graph API 配置访问评审的范围
description: 了解如何使用 Microsoft 应用商店中的访问评审 API Graph Azure AD 资源的访问权限。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: a4ed9b17d8d2b831071dc8f24e8330e595b543dc
ms.sourcegitcommit: 456ec9510807d05623c0ed1dd049c9676f53f56b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/22/2021
ms.locfileid: "53060292"
---
# <a name="configure-the-scope-of-your-access-review-using-the-microsoft-graph-api"></a><span data-ttu-id="d7d28-103">使用 Microsoft Graph API 配置访问评审的范围</span><span class="sxs-lookup"><span data-stu-id="d7d28-103">Configure the scope of your access review using the Microsoft Graph API</span></span>

<span data-ttu-id="d7d28-104">Azure AD [访问评审 API](/graph/api/resources/accessreviewsv2-root) 允许你以编程方式查看用户、服务主体或组对 Azure AD 资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="d7d28-104">The Azure AD [access reviews API](/graph/api/resources/accessreviewsv2-root) allows you to programmatically review the access that users, service principals, or groups have to your Azure AD resources.</span></span>

<span data-ttu-id="d7d28-105">要审阅的资源在访问评审 [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition)资源的 **scope** 属性中配置。</span><span class="sxs-lookup"><span data-stu-id="d7d28-105">The resources to review are configured in the **scope** property of the access reviews [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition) resource.</span></span> <span data-ttu-id="d7d28-106">此属性的类型为 [accessReviewScope，](/graph/api/resources/accessreviewscope)这是一个抽象类型，继承自以下资源，可用于配置将针对其访问的资源或资源组。</span><span class="sxs-lookup"><span data-stu-id="d7d28-106">This property is of the type [accessReviewScope](/graph/api/resources/accessreviewscope), an abstract type inherited by the following resources that can be used to configure resources or groups of resources that access will be reviewed against.</span></span>

|<span data-ttu-id="d7d28-107">资源</span><span class="sxs-lookup"><span data-stu-id="d7d28-107">Resource</span></span>|<span data-ttu-id="d7d28-108">说明</span><span class="sxs-lookup"><span data-stu-id="d7d28-108">Description</span></span>|<span data-ttu-id="d7d28-109">示例场景</span><span class="sxs-lookup"><span data-stu-id="d7d28-109">Example scenarios</span></span>|
|:---    |:---       |:---             |
|[<span data-ttu-id="d7d28-110">accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="d7d28-110">accessReviewQueryScope</span></span>](/graph/api/resources/accessreviewqueryscope)|<span data-ttu-id="d7d28-111">最适用于查看有权访问资源或相关资源组的完整主体集或子集。</span><span class="sxs-lookup"><span data-stu-id="d7d28-111">Best applicable when reviewing the full set or subset of principals who have access to a resource or group of related resources.</span></span>|<ul><li><span data-ttu-id="d7d28-112">分配给组的用户的成员身份。</span><span class="sxs-lookup"><span data-stu-id="d7d28-112">Membership of users assigned to a group.</span></span></li><li><span data-ttu-id="d7d28-113">来宾用户访问一个组。</span><span class="sxs-lookup"><span data-stu-id="d7d28-113">Guest user access to one group.</span></span></li><li><span data-ttu-id="d7d28-114">来宾用户访问租户Microsoft 365组。</span><span class="sxs-lookup"><span data-stu-id="d7d28-114">Guest user access to all Microsoft 365 groups in a tenant.</span></span></li><li><span data-ttu-id="d7d28-115">分配给特权角色的服务主体。</span><span class="sxs-lookup"><span data-stu-id="d7d28-115">Service principals assigned to privileged roles.</span></span></li><li><span data-ttu-id="d7d28-116">对权利管理访问包的用户和服务主体访问权限。</span><span class="sxs-lookup"><span data-stu-id="d7d28-116">User and service principal access to Entitlement Management access packages.</span></span></li></ul>|
|[<span data-ttu-id="d7d28-117">accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="d7d28-117">accessReviewInactiveUsersQueryScope</span></span>](/graph/api/resources/accessreviewinactiveusersqueryscope)|<span data-ttu-id="d7d28-118">继承自 accessReviewQueryScope。</span><span class="sxs-lookup"><span data-stu-id="d7d28-118">Inherited from accessReviewQueryScope.</span></span> <span data-ttu-id="d7d28-119">仅在查看非活动用户时使用。</span><span class="sxs-lookup"><span data-stu-id="d7d28-119">Used when only inactive users are reviewed.</span></span> <span data-ttu-id="d7d28-120">非活动状态由 **inactiveDuration 属性** 指定。</span><span class="sxs-lookup"><span data-stu-id="d7d28-120">Their inactive status is specified by the **inactiveDuration** property.</span></span> |<ul><li><span data-ttu-id="d7d28-121">仅非活动用户的组成员身份。</span><span class="sxs-lookup"><span data-stu-id="d7d28-121">Group membership of only inactive users.</span></span></li><ul>|
|[<span data-ttu-id="d7d28-122">principalResourceMembershipsScope</span><span class="sxs-lookup"><span data-stu-id="d7d28-122">principalResourceMembershipsScope</span></span>](/graph/api/resources/principalResourceMembershipsScope)|<span data-ttu-id="d7d28-123">最适用于查看主体对配置唯一主体和资源池的资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="d7d28-123">Best applicable to review principals' access to resources where you configure unique pools of principals and resources.</span></span>|<ul><li><span data-ttu-id="d7d28-124">查看跨 1 个组和 1 个特权 Azure AD 角色Microsoft 365 *3* 个特定主体的访问权限。</span><span class="sxs-lookup"><span data-stu-id="d7d28-124">Reviewing access of 3 specific principals across 1 Microsoft 365 group *and* 1 privileged Azure AD role.</span></span></li><ul>|

<span data-ttu-id="d7d28-125">本文将使用这些类型的 accessReviewScope 将各种 Azure AD 资源配置为访问评审的范围。</span><span class="sxs-lookup"><span data-stu-id="d7d28-125">In this article, you will use these types of accessReviewScope to configure a wide range of Azure AD resources as the scope of your access review.</span></span> <span data-ttu-id="d7d28-126">这可以帮助您自动执行主动审阅并控制对组织中资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="d7d28-126">This can help you to automate proactive review and keep control over access to resources in your organization.</span></span>  

## <a name="use-accessreviewqueryscope-to-configure-scope"></a><span data-ttu-id="d7d28-127">使用 accessReviewQueryScope 配置作用域</span><span class="sxs-lookup"><span data-stu-id="d7d28-127">Use accessReviewQueryScope to configure scope</span></span>

<span data-ttu-id="d7d28-128">若要使用 **accessReviewQueryScope** 类型配置范围，请设置其 **query、queryRoot** 和 **queryType** 属性的值。 </span><span class="sxs-lookup"><span data-stu-id="d7d28-128">To configure the scope by using the **accessReviewQueryScope** type, set the values of its **query**, **queryRoot**, and **queryType** properties.</span></span> <span data-ttu-id="d7d28-129">有关这些属性的说明，请参阅 [accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope) 资源类型。</span><span class="sxs-lookup"><span data-stu-id="d7d28-129">For descriptions of these properties, see [accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope) resource type.</span></span>

### <a name="example-1-review-all-users-assigned-to-a-group"></a><span data-ttu-id="d7d28-130">示例 1：查看分配给组的所有用户</span><span class="sxs-lookup"><span data-stu-id="d7d28-130">Example 1: Review all users assigned to a group</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
```
<span data-ttu-id="d7d28-131">若要仅 *查看分配给该组* 的非活动用户，请：</span><span class="sxs-lookup"><span data-stu-id="d7d28-131">To review *only inactive users* assigned to the group:</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "inactiveDuration": "P30D",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
````

### <a name="example-2-review-guest-users-assigned-to-a-group"></a><span data-ttu-id="d7d28-132">示例 2：查看分配给组的来宾用户</span><span class="sxs-lookup"><span data-stu-id="d7d28-132">Example 2: Review guest users assigned to a group</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",    
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-3-review-guest-users-assigned-to-all-microsoft-365-groups"></a><span data-ttu-id="d7d28-133">示例 3：查看分配给所有组Microsoft 365用户</span><span class="sxs-lookup"><span data-stu-id="d7d28-133">Example 3: Review guest users assigned to all Microsoft 365 groups</span></span>

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true ",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph"
}
```

<span data-ttu-id="d7d28-134">由于此审阅应用于所有Microsoft 365组，因此请配置 **instanceEnumerationScope** 以指定Microsoft 365组。</span><span class="sxs-lookup"><span data-stu-id="d7d28-134">Because this review is applied on all Microsoft 365 groups, configure the **instanceEnumerationScope** to specify the Microsoft 365 groups to review.</span></span>

### <a name="example-4-review-access-of-all-inactive-guest-users-to-all-groups"></a><span data-ttu-id="d7d28-135">示例 4：查看所有非活动来宾用户对全部组的访问权限</span><span class="sxs-lookup"><span data-stu-id="d7d28-135">Example 4: Review access of all inactive guest users to all groups</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

<span data-ttu-id="d7d28-136">由于此审阅适用于非活动用户，因此请使用 **accessReviewInactiveUsersQueryScope** 资源并使用值 指定 **@odata.type** 类型属性 `#microsoft.graph.accessReviewInactiveUsersQueryScope` 。</span><span class="sxs-lookup"><span data-stu-id="d7d28-136">Because this review is applied on inactive users, use the **accessReviewInactiveUsersQueryScope** resource and specify the **@odata.type** type property with the value `#microsoft.graph.accessReviewInactiveUsersQueryScope`.</span></span>

### <a name="example-5-review-of-all-inactive-guest-users-assigned-to-all-teams"></a><span data-ttu-id="d7d28-137">示例 5：查看分配给所有团队的所有非活动来宾用户</span><span class="sxs-lookup"><span data-stu-id="d7d28-137">Example 5: Review of all inactive guest users assigned to all teams</span></span>

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

<span data-ttu-id="d7d28-138">由于此审查适用于所有团队，因此请配置 **instanceEnumerationScope** 属性以指定所有团队。</span><span class="sxs-lookup"><span data-stu-id="d7d28-138">Because this review is applied on all teams, configure the **instanceEnumerationScope** property to specify all teams.</span></span>

### <a name="example-6-review-of-entitlement-management-access-package-assignment"></a><span data-ttu-id="d7d28-139">示例 6：审阅权利管理访问包分配</span><span class="sxs-lookup"><span data-stu-id="d7d28-139">Example 6: Review of Entitlement Management access package assignment</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')",
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-7-review-of-service-principals-assigned-to-privileged-roles"></a><span data-ttu-id="d7d28-140">示例 7：检查分配给特权角色的服务主体</span><span class="sxs-lookup"><span data-stu-id="d7d28-140">Example 7: Review of service principals assigned to privileged roles</span></span> 

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```

## <a name="use-principalresourcemembershipsscope-to-configure-scope"></a><span data-ttu-id="d7d28-141">使用 principalResourceMembershipsScope 配置作用域</span><span class="sxs-lookup"><span data-stu-id="d7d28-141">Use principalResourceMembershipsScope to configure scope</span></span>

<span data-ttu-id="d7d28-142">**principalResourceMembershipsScope** 公开 **principalScopes** 和 **resourceScopes** 属性，以支持 **针对 accessReviewScheduleDefinition** 作用域的更定制的配置选项。</span><span class="sxs-lookup"><span data-stu-id="d7d28-142">The **principalResourceMembershipsScope** exposes the **principalScopes** and **resourceScopes** properties to support more tailored configuration options for the scope of the **accessReviewScheduleDefinition**.</span></span> <span data-ttu-id="d7d28-143">这包括查看多个主体或主体组对多个资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="d7d28-143">This includes reviewing access for multiple principals or groups of principals to multiple resources.</span></span>

### <a name="example-1-review-access-of-all-inactive-guest-users-to-groups"></a><span data-ttu-id="d7d28-144">示例 1：查看所有非活动来宾用户对组的访问权限</span><span class="sxs-lookup"><span data-stu-id="d7d28-144">Example 1: Review access of all inactive guest users to groups</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
            "query": "/users?$filter=(userType eq 'Guest')",
            "queryType": "MicrosoftGraph",
            "inactiveDuration": "P30D"
        }
    ],
    "resourceScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/groups",
            "queryType": "MicrosoftGraph"
        }
    ]
}
```

<span data-ttu-id="d7d28-145">此示例中，主体是处于非活动状态的所有来宾用户，其不活动期计算为自访问评审实例的开始日期起 30 天。</span><span class="sxs-lookup"><span data-stu-id="d7d28-145">In this example, the principals are all inactive guest users with the period of their inactivity calculated as 30 days from the start date of the access review instance.</span></span>

### <a name="example-2-review-access-of-all-guest-users-to-a-directory-role"></a><span data-ttu-id="d7d28-146">示例 2：查看所有来宾用户对目录角色的访问权限</span><span class="sxs-lookup"><span data-stu-id="d7d28-146">Example 2: Review access of all guest users to a directory role</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/users?$filter=(userType eq 'Guest')",
            "queryType": "MicrosoftGraph"
        }
    ],
    "resourceScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/roleManagement/directory/roleDefinitions/{role id}",
            "queryType": "MicrosoftGraph"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="d7d28-147">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d7d28-147">See also</span></span>

+ [<span data-ttu-id="d7d28-148">向访问评审定义分配审阅者</span><span class="sxs-lookup"><span data-stu-id="d7d28-148">Assign reviewers to your access review definition</span></span>](/graph/accessreviews-reviewers-concept)
