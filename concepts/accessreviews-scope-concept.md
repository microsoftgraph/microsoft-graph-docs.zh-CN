---
title: 使用 Microsoft Graph API 配置访问评审定义的范围
description: 了解如何使用 Microsoft 应用商店中的访问评审 API Graph Azure AD 资源的访问权限。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: eff1d141d5c03190df4acedf7c3ed428d4cb24cd
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579809"
---
# <a name="configure-the-scope-of-your-access-review-definition-using-the-microsoft-graph-api"></a>使用 Microsoft Graph API 配置访问评审定义的范围

Azure AD [访问评审 API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true) 允许你以编程方式查看用户、服务主体或组对 Azure AD 资源的访问权限。

> [!NOTE]
> 访问[评审 API](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)仅适用于 Microsoft Graph beta 终结点。 请勿在生产应用中使用它，因为它可能会随时更改，恕不另行通知。

要审阅的资源在访问评审 [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition?view=graph-rest-beta&preserve-view=true)资源的 **scope** 属性中配置。 此属性的类型为 [accessReviewScope，](/graph/api/resources/accessreviewscope?view=graph-rest-beta&preserve-view=true)这是一个抽象类型，继承自以下资源，可用于配置将针对其访问的资源或资源组。

|资源|说明|示例场景|
|:---    |:---       |:---             |
|[accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope?view=graph-rest-beta&preserve-view=true)|最适用于查看有权访问资源或相关资源组的完整主体集或子集。|<ul><li>分配给组的用户的成员身份。</li><li>来宾用户访问一个组。</li><li>来宾用户访问租户Microsoft 365组。</li><li>分配给特权角色的服务主体。</li><li>对权利管理访问包的用户和服务主体访问权限。</li></ul>|
|[accessReviewInactiveUsersQueryScope](/graph/api/resources/accessreviewinactiveusersqueryscope?view=graph-rest-beta&preserve-view=true)|继承自 accessReviewQueryScope。 仅在查看非活动用户时使用。 非活动状态由 **inactiveDuration 属性** 指定。 |<ul><li>仅非活动用户的组成员身份。</li><ul>|
|[principalResourceMembershipsScope](/graph/api/resources/principalResourceMembershipsScope?view=graph-rest-beta&preserve-view=true)|最适用于查看主体对配置唯一主体和资源池的资源的访问权限。|<ul><li>查看跨 1 个组和 1 个特权 Azure AD 角色Microsoft 365 *3* 个特定主体的访问权限。</li><ul>|

本文将使用这些类型的 accessReviewScope 将各种 Azure AD 资源配置为访问评审的范围。 这可以帮助您自动执行主动审阅并控制对组织中资源的访问权限。  

## <a name="use-accessreviewqueryscope-to-configure-scope"></a>使用 accessReviewQueryScope 配置作用域

若要使用 **accessReviewQueryScope** 类型配置范围，请设置其 **query、queryRoot** 和 **queryType** 属性的值。  有关这些属性的说明，请参阅 [accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope?view=graph-rest-beta&preserve-view=true) 资源类型。

### <a name="example-1-review-all-users-assigned-to-a-group"></a>示例 1：查看分配给组的所有用户

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
```
若要仅 *查看分配给该组* 的非活动用户，请：

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "inactiveDuration": "P30D",
    "query": "/groups/{group id}/transitiveMembers",
    "queryType": "MicrosoftGraph"
}
````

### <a name="example-2-review-guest-users-assigned-to-a-group"></a>示例 2：查看分配给组的来宾用户

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",    
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-3-review-guest-users-assigned-to-all-microsoft-365-groups"></a>示例 3：查看分配给所有组Microsoft 365用户

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

由于此审阅应用于所有Microsoft 365组，因此请配置 **instanceEnumerationScope** 以指定Microsoft 365组。

### <a name="example-4-review-access-of-all-inactive-guest-users-to-all-groups"></a>示例 4：查看所有非活动来宾用户对全部组的访问权限

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

由于此审阅适用于非活动用户，因此请使用 **accessReviewInactiveUsersQueryScope** 资源并使用值 指定 **@odata.type** 类型属性 `#microsoft.graph.accessReviewInactiveUsersQueryScope` 。

### <a name="example-5-review-of-all-inactive-guest-users-assigned-to-all-teams"></a>示例 5：查看分配给所有团队的所有非活动来宾用户

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

由于此审查适用于所有团队，因此请配置 **instanceEnumerationScope** 属性以指定所有团队。

### <a name="example-6-review-of-entitlement-management-access-package-assignment"></a>示例 6：审阅权利管理访问包分配

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')",
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-7-review-of-service-principals-assigned-to-privileged-roles"></a>示例 7：检查分配给特权角色的服务主体 

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/beta/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```

## <a name="use-principalresourcemembershipsscope-to-configure-scope"></a>使用 principalResourceMembershipsScope 配置作用域

**principalResourceMembershipsScope** 公开 **principalScopes** 和 **resourceScopes** 属性，以支持 **针对 accessReviewScheduleDefinition** 作用域的更定制的配置选项。 这包括查看多个主体或主体组对多个资源的访问权限。

### <a name="example-1-review-access-of-all-inactive-guest-users-to-an-application"></a>示例 1：查看所有非活动来宾用户对应用程序的访问权限

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

此示例中，主体是处于非活动状态的所有来宾用户，其不活动期计算为自访问评审实例的开始日期起 30 天。

### <a name="example-2-review-access-of-all-guest-users-to-a-directory-role"></a>示例 2：查看所有来宾用户对目录角色的访问权限

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

## <a name="see-also"></a>另请参阅

+ [向访问评审定义分配审阅者](/graph/accessreviews-reviewers-concept)