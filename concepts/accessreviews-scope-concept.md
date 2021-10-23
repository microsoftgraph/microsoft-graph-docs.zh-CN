---
title: 使用 Microsoft Graph API 配置访问评审的范围
description: 了解如何使用 Microsoft 网站中的访问评审 API Graph查看对Azure AD的访问权限。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 3600d25e44e746f29c0a89950d1649ab5bef1a85
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2021
ms.locfileid: "60560735"
---
# <a name="configure-the-scope-of-your-access-review-using-the-microsoft-graph-api"></a>使用 Microsoft Graph API 配置访问评审的范围

通过Azure AD访问评审[API，](/graph/api/resources/accessreviewsv2-root)可以编程方式查看用户、服务主体或组对资源Azure AD的访问权限。

要审阅的资源在访问评审 [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition)资源的 **scope** 属性中配置。 此属性的类型为 [accessReviewScope，](/graph/api/resources/accessreviewscope)这是一个抽象类型，继承自以下资源，可用于配置将针对其访问的资源或资源组。

|资源|说明|示例场景|
|:---    |:---       |:---             |
|[accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope)|最适用于查看有权访问资源或相关资源组的完整主体集或子集。|<ul><li>分配给组的用户的成员身份。</li><li>来宾用户访问一个组。</li><li>来宾用户访问租户Microsoft 365组。</li><li>分配给特权角色的服务主体。</li><li>对权利管理访问包的用户和服务主体访问权限。</li></ul>|
|[accessReviewInactiveUsersQueryScope](/graph/api/resources/accessreviewinactiveusersqueryscope)|继承自 accessReviewQueryScope。 仅在查看非活动用户时使用。 非活动状态由 **inactiveDuration 属性** 指定。 |<ul><li>仅非活动用户的组成员身份。</li><ul>|
|[principalResourceMembershipsScope](/graph/api/resources/principalResourceMembershipsScope)|最适用于查看主体对配置唯一主体和资源池的资源的访问权限。|<ul><li>查看跨 1 个组和 1 个特权Microsoft 365 *3* 个特定Azure AD的访问权限。</li><ul>|

本文将介绍这些类型的 accessReviewScope，以配置各种Azure AD资源作为访问评审的范围。 这可以帮助您自动执行主动审阅并控制对组织中资源的访问权限。  

## <a name="use-accessreviewqueryscope-to-configure-scope"></a>使用 accessReviewQueryScope 配置作用域

若要使用 **accessReviewQueryScope** 类型配置范围，请设置其 **query、queryRoot** 和 **queryType** 属性的值。  有关这些属性的说明，请参阅 [accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope) 资源类型。

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
```

### <a name="example-2-review-all-guest-users-assigned-to-a-group"></a>示例 2：查看分配给组的所有来宾用户

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user/?$filter=(userType eq 'Guest')",    
    "queryType": "MicrosoftGraph"
}
```
### <a name="example-3-review-all-users-assigned-to-all-microsoft-365-groups"></a>示例 3：查看分配给所有组Microsoft 365用户

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified'))",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "./members/microsoft.graph.user",
    "queryType": "MicrosoftGraph"
}
```
由于此检查适用于所有Microsoft 365组，因此请配置 **instanceEnumerationScope** 以指定Microsoft 365组。 请注意，此审阅中不包含动态组和角色可分配组。

### <a name="example-4-review-all-guest-users-assigned-to-all-microsoft-365-groups"></a>示例 4：查看分配给所有来宾组的所有Microsoft 365用户

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified'))",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph"
}
```

由于此检查适用于所有Microsoft 365组，因此请配置 **instanceEnumerationScope** 以指定Microsoft 365组。 请注意，此审阅中不包含动态组和角色可分配组。
    
### <a name="example-5-review-all-guest-users-assigned-to-all-teams"></a>示例 5：查看分配给所有来宾组的所有来宾Teams

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph"
}
```
    
由于此审阅适用于所有Teams组Microsoft 365，因此请配置 **instanceEnumerationScope** 以指定Teams的Microsoft 365组。  请注意，此审阅中不包含动态组和角色可分配组。

### <a name="example-6-review-all-inactive-guest-users-assigned-to-all-microsoft-365-groups"></a>示例 6：查看分配给所有非活动来宾组的所有非Microsoft 365用户

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified'))",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

由于此审阅适用于非活动用户，请使用 **accessReviewInactiveUsersQueryScope** 资源并使用值 **指定 @odata.type** 类型属性 `#microsoft.graph.accessReviewInactiveUsersQueryScope` 。 请注意，此审阅中不包含动态组和角色可分配组。

### <a name="example-7-review-all-inactive-guest-users-assigned-to-all-teams"></a>示例 7：查看分配给所有用户的所有非活动来宾Teams

```http
"instanceEnumerationScope": {
    "query": "/groups?$filter=(groupTypes/any(c:c eq 'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
    "queryType": "MicrosoftGraph"
},
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
}
```

由于此审查适用于所有团队，因此请配置 **instanceEnumerationScope** 属性以指定所有团队。 请注意，此审阅中不包含动态组和角色可分配组。

### <a name="example-8-review-all-assignemnt-to-entitlement-management-access-packages"></a>示例 8：查看权利管理访问包的所有分配

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')",
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-9-review-all-service-principals-assigned-to-a-privileged-role"></a>示例 9：查看分配给特权角色的所有服务主体

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```
    
### <a name="example-10-review-all-users-assigned-to-a-privileged-role-all-active-and-eligible-assignments-included"></a>示例 10：查看分配给特权角色的所有用户 (包括的所有活动分配和符合条件的) 

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleDefinitions/{role ID}",
    "queryType": "MicrosoftGraph"
}
```
    
### <a name="example-11-review-all-users-with-eligible-assignment-to-a-privileged-role"></a>示例 11：查看具有特权角色的合格分配的所有用户

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleEligibilityScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.user') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```
    
### <a name="example-12-review-all-users-with-active-assignment-to-a-privileged-role"></a>示例 12：查看具有特权角色的活动分配的所有用户

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(assignmentType eq 'Assigned' and isof(principal,'microsoft.graph.user') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```

## <a name="use-principalresourcemembershipsscope-to-configure-scope"></a>使用 principalResourceMembershipsScope 配置作用域

**principalResourceMembershipsScope** 公开 **principalScopes** 和 **resourceScopes** 属性，以支持 **针对 accessReviewScheduleDefinition** 作用域的更定制的配置选项。 这包括查看多个主体或主体组对多个资源的访问权限。

### <a name="example-13-review-all-inactive-guest-users-assigned-to-all-groups"></a>示例 13：查看分配给所有组的所有非活动来宾用户

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

此示例中，主体是处于非活动状态的所有来宾用户，其不活动期计算为自访问评审实例的开始日期起 30 天。

### <a name="example-14-review-all-guest-users-assigned-to-a-directory-role"></a>示例 14：查看分配给目录角色的所有来宾用户

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

## <a name="next-steps"></a>后续步骤

+ [向访问评审定义分配审阅者](/graph/accessreviews-reviewers-concept)
+ [试用教程，](/graph/accessreviews-overview)了解如何使用访问评审 API 查看对Azure AD的访问权限
