---
title: 使用 Microsoft 图形 API配置访问评审的范围
description: 了解如何使用 Microsoft 图形 API 以编程方式查看用户、服务主体或组对 Azure AD 资源的访问权限。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 983bb98c9344fc745ebe9a36c27995cef4ce4562
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66698336"
---
# <a name="configure-the-scope-of-your-access-review-using-the-microsoft-graph-api"></a>使用 Microsoft 图形 API配置访问评审的范围

使用 Azure AD [访问评审 API](/graph/api/resources/accessreviewsv2-overview) ，可以以编程方式查看用户、服务主体或组对 Azure AD 资源的访问权限。 API 可帮助你自动执行主动评审并控制对组织中资源的访问。  

要审阅的资源在 [accessReviewScheduleDefinition](/graph/api/resources/accessreviewscheduledefinition) 资源 **的范围** 属性中配置。 此属性属于 [accessReviewScope](/graph/api/resources/accessreviewscope) 类型，这是可用于配置访问评审范围的以下 API 资源继承的抽象类型。

|资源|说明|示例场景|
|:---    |:---       |:---             |
|[accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope)|继承自 **accessReviewScope**。 查看有权访问资源或相关资源组的主体的完整集或子集时最适用。|<ul><li>分配给组的用户的成员身份（直接成员或直接成员和可传递成员）。</li><li>来宾用户对一个组的访问权限。</li><li>来宾用户访问租户中的所有 Microsoft 365 组。</li><li>分配给特权角色的服务主体。</li><li>用户和服务主体对权利管理访问包的访问权限。</li></ul>|
|[accessReviewInactiveUsersQueryScope](/graph/api/resources/accessreviewinactiveusersqueryscope)|继承自 **accessReviewQueryScope**。 仅审阅非活动用户时使用。 非活动状态由 **非活动重复** 属性指定。 |<ul><li>仅非活动用户的组成员身份。</li><ul>|
|[principalResourceMembershipsScope](/graph/api/resources/principalResourceMembershipsScope)|继承自 **accessReviewScope**。 最适用于查看主体对配置主体和资源的唯一池的资源的访问权限。|<ul><li>查看对一个 Microsoft 365 组 *和* 一个特权 Azure AD 角色的三个特定主体的访问权限。</li><ul>|

本文介绍如何使用这三种派生资源类型来限制访问评审的范围。

## <a name="use-accessreviewqueryscope-and-accessreviewinactiveusersqueryscope-to-configure-scope"></a>使用 accessReviewQueryScope 和 accessReviewInactiveUsersQueryScope 配置范围

若要使用 **accessReviewQueryScope** 类型配置范围，请设置其 **查询、****queryRoot** 和 **queryType** 属性的值。 有关这些属性的说明，请参阅 [accessReviewQueryScope](/graph/api/resources/accessreviewqueryscope) 资源类型。

**accessReviewInactiveUsersQueryScope** 需要 **accessReviewQueryScope** 的所有属性，并包含 **非活动性重复** 属性。

### <a name="example-1-review-all-users-assigned-to-a-group"></a>示例 1：查看分配给组的所有用户

下面的示例将评审范围限定为属于用户的组的直接成员和可传递成员。 可传递成员是嵌套组的成员。

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user",
    "queryType": "MicrosoftGraph"
}
```

**示例方案：** 假设组 A 有三个直接成员 - 用户 AU1 和 AU2 和组 G1。 另一方面，G1 组有两个成员 - 用户 GU1 和 GU2。 因此，用户 GU1 和 GU2 是嵌套组 G1 的可传递成员。 评审中将包含四个对象：用户 AU1、AU2、GU1 和 GU2。

仅查看分配给组的 *非活动用户* ：

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "inactiveDuration": "P30D",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user",
    "queryType": "MicrosoftGraph"
}
```

本示例还将评审范围限定到非活动用户组的直接成员和可传递成员。

### <a name="example-2-review-all-guest-users-assigned-to-a-group"></a>示例 2：查看分配给组的所有来宾用户

以下示例将评审范围限定到作为来宾用户的组的直接成员和可传递成员。 可传递成员是嵌套组的成员。

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/{group id}/transitiveMembers/microsoft.graph.user/?$filter=(userType eq 'Guest')",    
    "queryType": "MicrosoftGraph"
}
```

### <a name="example-3-review-all-users-and-groups-assigned-to-a-group"></a>示例 3：查看分配给组的所有用户和组

下面的示例将评审范围限定为仅将组的成员定向为用户或其他组。 在此范围内：
+ 直接用户包含在评审中。
+ 直接组包含在评审中。
+ 评审中不包括组的可传递成员（即嵌套组的成员）。

```http
"scope": {
        "query": "/groups/{group id}/members",
        "queryType": "MicrosoftGraph"
}
```

**示例方案：** 假设组 A 有三个直接成员 - 用户 AU1 和 AU2 和组 G1。 另一方面，G1 组有两个成员 - 用户 GU1 和 GU2。 因此，用户 GU1 和 GU2 是嵌套组 G1 的可传递成员。 在上述评审中，只有三个对象成为目标，用户是 AU1 和 AU2，以及组 G1。

### <a name="example-4-review-all-users-assigned-to-all-microsoft-365-groups"></a>示例 4：查看分配给所有 Microsoft 365 组的所有用户

以下示例创建对包含来宾用户的每个 Microsoft 365 组的评审。 对于每个组的审阅实例，评审范围仅限作为来宾用户的组的直接成员。

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

此外，由于此评审适用于所有 Microsoft 365 组，因此请将 **instanceEnumerationScope** 配置为指定要审阅的 Microsoft 365 组。 此评审中不包括动态组和可分配角色的组。

### <a name="example-5-review-all-guest-users-assigned-to-all-microsoft-365-groups"></a>示例 5：查看分配给所有 Microsoft 365 组的所有来宾用户

以下示例将评审范围限定到所有作为来宾用户的 Microsoft 365 组的成员。

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

此外，由于此评审适用于所有 Microsoft 365 组，因此请将 **instanceEnumerationScope** 配置为指定要审阅的 Microsoft 365 组。 此评审中不包括动态组和可分配角色的组。

#### <a name="review-all-inactive-guest-users-assigned-to-all-microsoft-365-groups"></a>查看分配给所有 Microsoft 365 组的所有非活动来宾用户

以下示例将评审范围限定为所有非活动来宾用户的所有 Microsoft 365 成员。

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

此外，由于此评审应用于非活动用户，请使用 **accessReviewInactiveUsersQueryScope** 资源并指定具有值`#microsoft.graph.accessReviewInactiveUsersQueryScope`**的 @odata.type** 属性。 此评审中不包括动态组和可分配角色的组。

### <a name="example-6-review-all-guest-users-assigned-to-all-teams"></a>示例 6：查看分配给所有团队的所有来宾用户

以下示例将评审范围限定为指导作为来宾用户的所有团队的成员。

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
    
此外，由于此评审适用于所有已启用 Teams 的 Microsoft 365 组，因此请将 **instanceEnumerationScope** 配置为指定启用 Teams 的 Microsoft 365 组以进行评审。 此评审中不包括动态组和可分配角色的组。

此评审不包括具有共享频道的团队中的 B2B 直接连接用户。 若要在具有共享频道的团队中包括 B2B 直接连接用户，请参阅 [示例 11：查看分配给团队的所有用户，包括具有共享频道的团队中的 B2B 直接连接用户](#example-11-review-all-users-assigned-to-a-team-including-b2b-direct-connect-users-in-a-team-with-shared-channels)。

#### <a name="review-all-inactive-guest-users-assigned-to-all-teams"></a>查看分配给所有 Teams 的所有非活动来宾用户

以下示例将评审范围限定为指导非活动来宾用户的所有团队的成员。

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

此外，由于此评审适用于所有团队，因此请将 **instanceEnumerationScope** 属性配置为指定所有团队。 此评审中不包括动态组和可分配角色的组。

此评审不包括具有共享频道的团队中的 B2B 直接连接用户。 若要在具有共享频道的团队中包括 B2B 直接连接用户，请参阅 [示例 11：查看分配给团队的所有用户，包括具有共享频道的团队中的 B2B 直接连接用户](#example-11-review-all-users-assigned-to-a-team-including-b2b-direct-connect-users-in-a-team-with-shared-channels)。

---

### <a name="example-7-review-all-assignment-to-entitlement-management-access-packages"></a>示例 7：查看权利管理访问包的所有分配

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/identityGovernance/entitlementManagement/accessPackageAssignments?$filter=(accessPackageId eq '{package id}' and assignmentPolicyId eq '{id}')",
    "queryType": "MicrosoftGraph"
}
```

---

### <a name="example-8-review-all-service-principals-assigned-to-a-privileged-role"></a>示例 8：查看分配给特权角色的所有服务主体

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.servicePrincipal') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```
    
### <a name="example-9-review-all-users-assigned-to-a-privileged-role"></a>示例 9：查看分配给特权角色的所有用户 

#### <a name="review-all-users-assigned-to-a-privileged-role-all-active-and-eligible-assignments-included"></a>查看分配给特权角色的所有用户 (包含的所有活动和符合条件的分配) 

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleDefinitions/{role ID}",
    "queryType": "MicrosoftGraph"
}
```
    
#### <a name="review-all-users-with-eligible-assignment-to-a-privileged-role"></a>查看具有特权角色的合格分配的所有用户

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleEligibilityScheduleInstances?$expand=principal&$filter=(isof(principal,'microsoft.graph.user') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```
    
#### <a name="review-all-users-with-active-assignment-to-a-privileged-role"></a>查看具有特权角色的活动分配的所有用户

```http
"scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/roleManagement/directory/roleAssignmentScheduleInstances?$expand=principal&$filter=(assignmentType eq 'Assigned' and isof(principal,'microsoft.graph.user') and roleDefinitionId eq '{role ID}')",
    "queryType": "MicrosoftGraph"
}
```

---

## <a name="use-principalresourcemembershipsscope-to-configure-scope"></a>使用 principalResourceMembershipsScope 配置范围

**principalResourceMembershipsScope** 公开 **principalScopes** 和 **resourceScopes** 属性，以支持 **accessReviewScheduleDefinition** 对象范围的更多定制配置选项。 这些功能包括查看多个主体或主体组对多个资源的访问权限。

### <a name="example-10-review-all-inactive-guest-users-assigned-to-all-groups"></a>示例 10：查看分配给所有组的所有非活动来宾用户

以下示例将评审范围限定到非活动来宾用户的所有组的成员。 当来宾用户的非活动期为访问评审实例开始日期的 30 天时，将被视为非活动用户。

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

### <a name="example-11-review-all-users-assigned-to-a-team-including-b2b-direct-connect-users-in-a-team-with-shared-channels"></a>示例 11：查看分配给团队的所有用户，包括具有共享频道的团队中的 B2B 直接连接用户

在此示例中，访问评审范围是团队成员或分配到团队内共享频道的所有用户。 这些成员包括内部用户、直接和可传递用户、B2B 协作用户和 B2B 直接连接用户。

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
            "query": "/groups/{groupId}/transitiveMembers/microsoft.graph.user",
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

若要查看共享通道中的 B2B 直接连接用户和团队，必须在 **resourceScopes** 对象中指定`/teams/{groupId}/channels?$filter=(membershipType eq 'shared')`**查询** 模式。 *所有团队* 评审（例如 [示例 6](#review-all-inactive-guest-users-assigned-to-all-teams)）不会在共享通道中包含 B2B 直接连接用户和团队。

> [!NOTE]
> B2B 直接连接用户和团队的访问评审仅在单阶段访问评审中受支持，而在多阶段访问评审中不受支持。

### <a name="example-12-review-all-guest-users-assigned-to-a-directory-role"></a>示例 12：查看分配给目录角色的所有来宾用户

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

+ [将审阅者分配到访问评审定义](/graph/accessreviews-reviewers-concept)
+ [试用教程](/graph/accessreviews-overview) ，了解如何使用访问评审 API 来评审对 Azure AD 资源的访问权限
+ [创建访问评审](/azure/active-directory/governance/create-access-review)
