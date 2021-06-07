---
title: 使用 Microsoft Graph API 配置访问评审的范围
description: 了解如何使用 Microsoft 应用商店中的访问评审 API Graph Azure AD 资源的访问权限。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: fe61a015ab88e5e3c562b8837d57b997400f8ed3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755628"
---
# <a name="configure-the-scope-of-your-access-review-using-the-microsoft-graph-api"></a><span data-ttu-id="40894-103">使用 Microsoft Graph API 配置访问评审的范围</span><span class="sxs-lookup"><span data-stu-id="40894-103">Configure the scope of your access review using the Microsoft Graph API</span></span>

<span data-ttu-id="40894-104">Azure AD [访问评审 API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) 允许你以编程方式查看用户、服务主体或组对 Azure AD 资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="40894-104">The Azure AD [access reviews API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) allows you to programmatically review the access that users, service principals, or groups have to your Azure AD resources.</span></span>

> [!NOTE]
> <span data-ttu-id="40894-105">访问[评审 API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)仅适用于 Microsoft Graph beta 终结点。</span><span class="sxs-lookup"><span data-stu-id="40894-105">The [access reviews API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) is available in only the Microsoft Graph beta endpoint.</span></span> <span data-ttu-id="40894-106">请勿在生产应用中使用它，因为它可能会随时更改，恕不另行通知。</span><span class="sxs-lookup"><span data-stu-id="40894-106">Do not use it in production apps, as it is subject to change without notice.</span></span>

<span data-ttu-id="40894-107">要审阅的资源在访问评审 [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true)资源的 **scope** 属性中配置。</span><span class="sxs-lookup"><span data-stu-id="40894-107">The resources to review are configured in the **scope** property of the access reviews [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true) resource.</span></span> <span data-ttu-id="40894-108">此属性的类型为 [accessReviewScope，](/graph/api/resources/accessreviewscope?view=graph-rest-beta&preserve-view=true)这是一个抽象类型，继承自以下资源，可用于配置将针对其访问的资源或资源组。</span><span class="sxs-lookup"><span data-stu-id="40894-108">This property is of the type [accessReviewScope](/graph/api/resources/accessreviewscope?view=graph-rest-beta&preserve-view=true), an abstract type inherited by the following resources that can be used to configure resources or groups of resources that access will be reviewed against.</span></span>

|<span data-ttu-id="40894-109">资源</span><span class="sxs-lookup"><span data-stu-id="40894-109">Resource</span></span>|<span data-ttu-id="40894-110">说明</span><span class="sxs-lookup"><span data-stu-id="40894-110">Description</span></span>|<span data-ttu-id="40894-111">示例场景</span><span class="sxs-lookup"><span data-stu-id="40894-111">Example scenarios</span></span>|
|:---    |:---       |:---             |
|[<span data-ttu-id="40894-112">accessReviewQueryScope</span><span class="sxs-lookup"><span data-stu-id="40894-112">accessReviewQueryScope</span></span>](/graph/api/resources/accessreviewqueryscope?view=graph-rest-beta&preserve-view=true)|<span data-ttu-id="40894-113">最适用于查看有权访问资源或相关资源组的完整主体集或子集。</span><span class="sxs-lookup"><span data-stu-id="40894-113">Best applicable when reviewing the full set or subset of principals who have access to a resource or group of related resources.</span></span>|<ul><li><span data-ttu-id="40894-114">分配给组的用户的成员身份。</span><span class="sxs-lookup"><span data-stu-id="40894-114">Membership of users assigned to a group.</span></span></li><li><span data-ttu-id="40894-115">来宾用户访问一个组。</span><span class="sxs-lookup"><span data-stu-id="40894-115">Guest user access to one group.</span></span></li><li><span data-ttu-id="40894-116">来宾用户访问租户Microsoft 365组。</span><span class="sxs-lookup"><span data-stu-id="40894-116">Guest user access to all Microsoft 365 groups in a tenant.</span></span></li><li><span data-ttu-id="40894-117">分配给特权角色的服务主体。</span><span class="sxs-lookup"><span data-stu-id="40894-117">Service principals assigned to privileged roles.</span></span></li><li><span data-ttu-id="40894-118">对权利管理访问包的用户和服务主体访问权限。</span><span class="sxs-lookup"><span data-stu-id="40894-118">User and service principal access to Entitlement Management access packages.</span></span></li></ul>|
|[<span data-ttu-id="40894-119">accessReviewInactiveUsersQueryScope</span><span class="sxs-lookup"><span data-stu-id="40894-119">accessReviewInactiveUsersQueryScope</span></span>](/graph/api/resources/accessreviewinactiveusersqueryscope?view=graph-rest-beta&preserve-view=true)|<span data-ttu-id="40894-120">继承自 accessReviewQueryScope。</span><span class="sxs-lookup"><span data-stu-id="40894-120">Inherited from accessReviewQueryScope.</span></span> <span data-ttu-id="40894-121">仅在查看非活动用户时使用。</span><span class="sxs-lookup"><span data-stu-id="40894-121">Used when only inactive users are reviewed.</span></span> <span data-ttu-id="40894-122">非活动状态由 **inactiveDuration 属性** 指定。</span><span class="sxs-lookup"><span data-stu-id="40894-122">Their inactive status is specified by the **inactiveDuration** property.</span></span> |<ul><li><span data-ttu-id="40894-123">仅非活动用户的组成员身份。</span><span class="sxs-lookup"><span data-stu-id="40894-123">Group membership of only inactive users.</span></span></li><ul>|
|[<span data-ttu-id="40894-124">principalResourceMembershipsScope</span><span class="sxs-lookup"><span data-stu-id="40894-124">principalResourceMembershipsScope</span></span>](/graph/api/resources/principalResourceMembershipsScope?view=graph-rest-beta&preserve-view=true)|<span data-ttu-id="40894-125">最适用于查看主体对配置唯一主体和资源池的资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="40894-125">Best applicable to review principals' access to resources where you configure unique pools of principals and resources.</span></span>|<ul><li><span data-ttu-id="40894-126">查看跨 1 个组和 1 个特权 Azure AD 角色Microsoft 365 *3* 个特定主体的访问权限。</span><span class="sxs-lookup"><span data-stu-id="40894-126">Reviewing access of 3 specific principals across 1 Microsoft 365 group *and* 1 privileged Azure AD role.</span></span></li><ul>|

<span data-ttu-id="40894-127">本文将使用这些类型的 accessReviewScope 将各种 Azure AD 资源配置为访问评审的范围。</span><span class="sxs-lookup"><span data-stu-id="40894-127">In this article, you will use these types of accessReviewScope to configure a wide range of Azure AD resources as the scope of your access review.</span></span> <span data-ttu-id="40894-128">这可以帮助您自动执行主动审阅并控制对组织中资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="40894-128">This can help you to automate proactive review and keep control over access to resources in your organization.</span></span>  

## <a name="use-accessreviewqueryscope-to-configure-scope"></a><span data-ttu-id="40894-129">使用 accessReviewQueryScope 配置作用域</span><span class="sxs-lookup"><span data-stu-id="40894-129">Use accessReviewQueryScope to configure scope</span></span>

<span data-ttu-id="40894-130">若要使用 **accessReviewQueryScope** 类型配置范围，请设置其 **query、queryRoot** 和 **queryType** 属性的值。 </span><span class="sxs-lookup"><span data-stu-id="40894-130">To configure the scope by using the **accessReviewQueryScope** type, set the values of its **query**, **queryRoot**, and **queryType** properties.</span></span> <span data-ttu-id="40894-131">有关这些属性的说明，请参阅 [accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope?view=graph-rest-beta&preserve-view=true) 资源类型。</span><span class="sxs-lookup"><span data-stu-id="40894-131">For descriptions of these properties, see [accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope?view=graph-rest-beta&preserve-view=true) resource type.</span></span>

### <a name="example-1-review-all-users-assigned-to-a-group"></a><span data-ttu-id="40894-132">示例 1：查看分配给组的所有用户</span><span class="sxs-lookup"><span data-stu-id="40894-132">Example 1: Review all users assigned to a group</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
```
<span data-ttu-id="40894-133">若要仅 *查看分配给该组* 的非活动用户，请：</span><span class="sxs-lookup"><span data-stu-id="40894-133">To review *only inactive users* assigned to the group:</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "inactiveDuration": "P30D",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
````

### <a name="example-2-review-guest-users-assigned-to-a-group"></a><span data-ttu-id="40894-134">示例 2：查看分配给组的来宾用户</span><span class="sxs-lookup"><span data-stu-id="40894-134">Example 2: Review guest users assigned to a group</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",    
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-3-review-guest-users-assigned-to-all-microsoft-365-groups"></a><span data-ttu-id="40894-135">示例 3：查看分配给所有组Microsoft 365用户</span><span class="sxs-lookup"><span data-stu-id="40894-135">Example 3: Review guest users assigned to all Microsoft 365 groups</span></span>

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

<span data-ttu-id="40894-136">由于此审阅应用于所有Microsoft 365组，因此请配置 **instanceEnumerationScope** 以指定Microsoft 365组。</span><span class="sxs-lookup"><span data-stu-id="40894-136">Because this review is applied on all Microsoft 365 groups, configure the **instanceEnumerationScope** to specify the Microsoft 365 groups to review.</span></span>

### <a name="example-4-review-access-of-all-inactive-guest-users-to-all-groups"></a><span data-ttu-id="40894-137">示例 4：查看所有非活动来宾用户对全部组的访问权限</span><span class="sxs-lookup"><span data-stu-id="40894-137">Example 4: Review access of all inactive guest users to all groups</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

<span data-ttu-id="40894-138">由于此审阅适用于非活动用户，因此请使用 **accessReviewInactiveUsersQueryScope** 资源并使用值 指定 **@odata.type** 类型属性 `#microsoft.graph.accessReviewInactiveUsersQueryScope` 。</span><span class="sxs-lookup"><span data-stu-id="40894-138">Because this review is applied on inactive users, use the **accessReviewInactiveUsersQueryScope** resource and specify the **@odata.type** type property with the value `#microsoft.graph.accessReviewInactiveUsersQueryScope`.</span></span>

### <a name="example-5-review-of-all-inactive-guest-users-assigned-to-all-teams"></a><span data-ttu-id="40894-139">示例 5：查看分配给所有团队的所有非活动来宾用户</span><span class="sxs-lookup"><span data-stu-id="40894-139">Example 5: Review of all inactive guest users assigned to all teams</span></span>

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

<span data-ttu-id="40894-140">由于此审查适用于所有团队，因此请配置 **instanceEnumerationScope** 属性以指定所有团队。</span><span class="sxs-lookup"><span data-stu-id="40894-140">Because this review is applied on all teams, configure the **instanceEnumerationScope** property to specify all teams.</span></span>

### <a name="example-6-review-of-entitlement-management-access-package-assignment"></a><span data-ttu-id="40894-141">示例 6：审阅权利管理访问包分配</span><span class="sxs-lookup"><span data-stu-id="40894-141">Example 6: Review of Entitlement Management access package assignment</span></span>

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')",
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-7-review-of-service-principals-assigned-to-privileged-roles"></a><span data-ttu-id="40894-142">示例 7：检查分配给特权角色的服务主体</span><span class="sxs-lookup"><span data-stu-id="40894-142">Example 7: Review of service principals assigned to privileged roles</span></span> 

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/beta/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```

## <a name="use-principalresourcemembershipsscope-to-configure-scope"></a><span data-ttu-id="40894-143">使用 principalResourceMembershipsScope 配置作用域</span><span class="sxs-lookup"><span data-stu-id="40894-143">Use principalResourceMembershipsScope to configure scope</span></span>

<span data-ttu-id="40894-144">**principalResourceMembershipsScope** 公开 **principalScopes** 和 **resourceScopes** 属性，以支持 **针对 accessReviewScheduleDefinition** 作用域的更定制的配置选项。</span><span class="sxs-lookup"><span data-stu-id="40894-144">The **principalResourceMembershipsScope** exposes the **principalScopes** and **resourceScopes** properties to support more tailored configuration options for the scope of the **accessReviewScheduleDefinition**.</span></span> <span data-ttu-id="40894-145">这包括查看多个主体或主体组对多个资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="40894-145">This includes reviewing access for multiple principals or groups of principals to multiple resources.</span></span>

### <a name="example-1-review-access-of-all-inactive-guest-users-to-an-application"></a><span data-ttu-id="40894-146">示例 1：查看所有非活动来宾用户对应用程序的访问权限</span><span class="sxs-lookup"><span data-stu-id="40894-146">Example 1: Review access of all inactive guest users to an application</span></span>

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
            "query": "/servicePrincipals/{serviceprincipal id}",
            "queryType": "MicrosoftGraph"
        }
    ]
}
```

<span data-ttu-id="40894-147">此示例中，主体是处于非活动状态的所有来宾用户，其不活动期计算为自访问评审实例的开始日期起 30 天。</span><span class="sxs-lookup"><span data-stu-id="40894-147">In this example, the principals are all inactive guest users with the period of their inactivity calculated as 30 days from the start date of the access review instance.</span></span>

### <a name="example-2-review-access-of-all-guest-users-to-a-directory-role"></a><span data-ttu-id="40894-148">示例 2：查看所有来宾用户对目录角色的访问权限</span><span class="sxs-lookup"><span data-stu-id="40894-148">Example 2: Review access of all guest users to a directory role</span></span>

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

## <a name="see-also"></a><span data-ttu-id="40894-149">另请参阅</span><span class="sxs-lookup"><span data-stu-id="40894-149">See also</span></span>

+ [<span data-ttu-id="40894-150">向访问评审定义分配审阅者</span><span class="sxs-lookup"><span data-stu-id="40894-150">Assign reviewers to your access review definition</span></span>](/graph/accessreviews-reviewers-concept)