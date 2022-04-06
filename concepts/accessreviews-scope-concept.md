---
title: 使用 Microsoft 网站配置访问评审图形 API
description: 了解如何使用 Microsoft 网站中的访问评审 API Graph查看对Azure AD的访问权限。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 4d1439e2086934ad01fcc83978b70c6dc68b083c
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2022
ms.locfileid: "64509915"
---
# <a name="configure-the-scope-of-your-access-review-using-the-microsoft-graph-api"></a>使用 Microsoft 网站配置访问评审图形 API

访问Azure AD [API](/graph/api/resources/accessreviewsv2-overview) 允许你以编程方式查看用户、服务主体或组对访问你的Azure AD的访问权限。

要审阅的资源在访问评审 [accessReviewScheduleDefinition 资源的 scope 属性中](/graph/api/resources/accessreviewscheduledefinition)配置。 此属性的类型为 [accessReviewScope](/graph/api/resources/accessreviewscope)，这是一个抽象类型，继承自以下资源，可用于配置将针对其访问的资源或资源组。

|资源|说明|示例场景|
|:---    |:---       |:---             |
|[accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope)|最适用于查看有权访问资源或相关资源组的完整主体集或子集。|<ul><li>分配给组的用户的成员身份。</li><li>来宾用户访问一个组。</li><li>来宾用户对租户中Microsoft 365组的访问权限。</li><li>分配给特权角色的服务主体。</li><li>对权利管理访问包的用户和服务主体访问权限。</li></ul>|
|[accessReviewInactiveUsersQueryScope](/graph/api/resources/accessreviewinactiveusersqueryscope)|继承自 accessReviewQueryScope。 仅在查看非活动用户时使用。 非活动状态由 **inactiveDuration 属性** 指定。 |<ul><li>仅非活动用户的组成员身份。</li><ul>|
|[principalResourceMembershipsScope](/graph/api/resources/principalResourceMembershipsScope)|最适用于查看主体对配置唯一主体和资源池的资源的访问权限。|<ul><li>查看跨 1 个组 3 个特定主体Microsoft 365 *1 个特权* Azure AD角色。</li><ul>|

本文将介绍这些类型的 accessReviewScope，以配置各种Azure AD资源作为访问评审的范围。 这可以帮助您自动执行主动审阅并控制对组织中资源的访问权限。  

## <a name="use-accessreviewqueryscope-to-configure-scope"></a>使用 accessReviewQueryScope 配置作用域

若要使用 **accessReviewQueryScope** 类型配置范围，请设置其 **query**、 **queryRoot** 和 **queryType** 属性的值。 有关这些属性的说明，请参阅 [accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope) 资源类型。

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

### <a name="example-3-review-all-users-assigned-to-all-microsoft-365-groups"></a>示例 3：查看分配给所有组的所有Microsoft 365用户

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

### <a name="example-5-review-all-guest-users-assigned-to-all-teams"></a>示例 5：查看分配给所有用户的所有来宾Teams

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
    
由于此审查适用于所有Teams组Microsoft 365，因此请配置 **instanceEnumerationScope** 以指定Teams的Microsoft 365组。  请注意，此审阅中不包含动态组和角色可分配组。

此评论不包括使用共享频道的团队中的 B2B 直接连接用户。 若要在具有共享频道的团队中包括 B2B 直接连接用户，请参阅示例 14：查看分配给团队的所有用户，包括使用共享频道的团队中的 [B2B](#example-14-review-all-users-assigned-to-a-team-including-b2b-direct-connect-users-in-a-team-with-shared-channels) 直接连接用户。

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

由于此审阅适用于非活动用户，请使用 **accessReviewInactiveUsersQueryScope** 资源并使用值 **指定 @odata.type** 类型属性 `#microsoft.graph.accessReviewInactiveUsersQueryScope`。 请注意，此审阅中不包含动态组和角色可分配组。

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

此评论不包括使用共享频道的团队中的 B2B 直接连接用户。 若要在具有共享频道的团队中包括 B2B 直接连接用户，请参阅示例 14：查看分配给团队的所有用户，包括使用共享频道的团队中的 [B2B](#example-14-review-all-users-assigned-to-a-team-including-b2b-direct-connect-users-in-a-team-with-shared-channels) 直接连接用户。

### <a name="example-8-review-all-assignment-to-entitlement-management-access-packages"></a>示例 8：查看对权利管理访问包的所有分配

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

本示例中，主体是处于非活动状态的所有来宾用户，其不活动期计算为自访问评审实例的开始日期起 30 天。

### <a name="example-14-review-all-users-assigned-to-a-team-including-b2b-direct-connect-users-in-a-team-with-shared-channels"></a>示例 14：查看分配给团队的所有用户，包括使用共享频道直接连接团队中的用户

```http
"scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/users",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "resourceScopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/groups/{groupId}/transitiveMembers",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        },
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/teams/{groupId}/channels?$filter=(membershipType eq 'shared')",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ]
}
```

本示例中，访问评审的范围为属于团队成员或分配到团队内共享频道的所有用户，包括内部用户、B2B 协作用户和 B2B 直接连接用户。

若要查看共享频道中的 B2B `/teams/{groupId}/channels?$filter=(membershipType eq 'shared')` 直接连接用户和团队，必须在 **resourceScopes** 对象中指定查询模式。 所有 *团队* 评审（如示例 [7](#example-5-review-all-guest-users-assigned-to-all-teams)）不会在共享频道中包括 B2B 直接连接用户和团队。

> [!NOTE]
> B2B 直接连接用户和团队的访问评审仅在单阶段访问评审中受支持，在多阶段访问评审中不受支持。

### <a name="example-15-review-all-guest-users-assigned-to-a-directory-role"></a>示例 15：查看分配给目录角色的所有来宾用户

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
+ [创建访问评审](/azure/active-directory/governance/create-access-review)
