---
title: 教程：使用访问评审 API 查看对特权角色的访问权限
description: 了解如何使用访问评审 API 定期查看有权访问特权角色的用户和组，包括活动角色和符合条件的角色。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 845d50d4cd3eb06cf2131f5255567cb4b7861325
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445809"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-access-to-privileged-roles"></a>教程：使用访问评审 API 查看对特权角色的访问权限

Microsoft Graph 中的访问评审 API 使组织能够审核和证明标识 (也称为 *主体*) 分配给组织中资源的访问权限。 组织中最敏感的资源之一是特权角色。 使用特权角色，主体可以执行管理操作。 根据特权角色，某些操作可能会对组织的安全状况产生更大的影响。 使用访问评审 API，组织可以根据组织策略定期证明有权访问特权角色的主体。

Contoso Limited 是一家不断增长的服务提供商，已将各种 Azure AD 管理员权限委派给组织中的用户、组和服务主体。 公司需要确保只有合适的被分配者才有权访问特权角色。 系统审核员还应审核访问评审历史记录，以报告 Contoso 内部控制措施的有效性。

在本教程中，你将使用访问评审 API 定期查看有权访问 Contoso 中特权角色的用户和组。 此访问包括活动角色和符合条件的角色。

## <a name="prerequisites"></a>先决条件

若要完成本教程，需要以下资源和权限：

+ 已启用Azure AD Premium P2或 EMS E5 许可证的工作 Azure AD 租户。
+ 以特权角色管理员角色中的用户身份登录到 [Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer) 。
+ 具有特权角色的活动或符合条件分配的主体。 这些分配将是访问评审的范围。 若要分配特权角色，请参阅[教程：使用 Privileged Identity Management (PIM) API 分配 Azure AD 角色](/graph/tutorial-assign-azureadroles)。
    + 在本教程中，用户管理员角色是正在评审的资源。 已为安全组和单个用户分配该角色。
+ 以下委派权限： `AccessReview.ReadWrite.All`.

若要在 Graph 资源管理器中同意所需权限，请执行以下操作：
1. 选择用户帐户详细信息右侧的水平省略号图标，然后选择 **“选择权限**”。

      :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="选择 Microsoft Graph 权限。" border="true":::

2. 滚动浏览 **AccessReview (3)** 的权限列表，展开然后选择 `AccessReview.ReadWrite.All`。 选择“**同意**”，然后选择“**接受**”，以接受同意权限。

      :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="同意 Microsoft Graph 权限。" border="true":::

>[!NOTE]
>本教程中显示的响应对象可能会缩短以实现可读性。

## <a name="step-1-create-an-access-review-of-privileged-role-assignments"></a>步骤 1：创建特权角色分配的访问评审

在本教程中，我们将针对用户管理员角色的 *活动* 和 *符合条件* 的分配创建定期访问评审。 **accessReviewScheduleDefinition** 可用于定义对多个主体类型的访问评审， (用户和组，或服务主体) 只有一个特权角色。 若要查看对多个特权角色的访问权限，请创建单独 **的 accessReviewScheduleDefinition** 对象。

以下访问评审计划定义具有以下设置：

+ 评审范围是主体 (**principalScopes** 属性) ，可访问 **resourceScopes** 属性中指定的资源。 在这种情况下，主体是组和用户，而资源是用户管理员角色。
+ 正在审查对用户管理员角色资源的活动分配和符合条件的分配。
+ 选择单个用户作为审阅者。 在此示例中，你将成为审阅者。
+ 审批者必须先提供理由，然后才能批准对特权角色的访问权限。
+ 默认决策是在 `None` 实例过期之前审阅者不响应访问评审请求时作出的。
+ **未将 autoApplyDecisionsEnabled** 设置为默认 `false`值。 在这种情况下，审阅完成后，不会自动应用决策，因此必须手动应用这些决策。
+ 评审在三天内每三个月重复一次，但不会结束。

### <a name="request"></a>请求

在以下请求中 `f674a1c9-4a40-439c-bfa3-4b61a9f29d85` ，替换为用户 ID 的值。 roleDefinitionId `fe930be7-5e62-47db-91af-98c3a49a38b1` 是 Azure AD 中用户管理员角色的全局模板标识符。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviledroles-create"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "Review access of users and groups to privileged roles",
    "descriptionForAdmins": "Review access of users and groups to privileged roles",
    "scope": {
        "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
        "principalScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/users",
                "queryType": "MicrosoftGraph"
            },
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/groups",
                "queryType": "MicrosoftGraph"
            }
        ],
        "resourceScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
                "queryType": "MicrosoftGraph"
            }
        ]
    },
    "reviewers": [
        {
            "query": "/users/f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
            "queryType": "MicrosoftGraph"
        }
    ],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 3,
        "recommendationsEnabled": false,
        "recurrence": {
            "pattern": {
                "type": "absoluteMonthly",
                "interval": 3
            },
            "range": {
                "type": "noEnd",
                "startDate": "2022-03-02"
            }
        }
    }
}
```

### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions/$entity",
    "id": "57457d7c-af59-470c-ae71-aa72c657fe0f",
    "displayName": "Review access of users and groups to privileged roles",
    "createdDateTime": null,
    "lastModifiedDateTime": null,
    "status": "NotStarted",
    "descriptionForAdmins": "Review access of users and groups to privileged roles",
    "descriptionForReviewers": null,
    "instanceEnumerationScope": null,
    "createdBy": {
        "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
        "displayName": "Alex Wilber",
        "type": null,
        "userPrincipalName": "AlexW@Contoso.com"
    },
    "scope": {
        "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
        "principalScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/users",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/groups",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        ],
        "resourceScopes": [
            {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/roleManagement/directory/roleDefinitions/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        ]
    },
    "reviewers": [
        {
            "query": "/users/f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "fallbackReviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": false,
        "defaultDecision": "None",
        "instanceDurationInDays": 3,
        "autoApplyDecisionsEnabled": false,
        "recommendationsEnabled": false,
        "recurrence": {
            "pattern": {
                "type": "absoluteMonthly",
                "interval": 3,
                "month": 0,
                "dayOfMonth": 0,
                "daysOfWeek": [],
                "firstDayOfWeek": "sunday",
                "index": "first"
            },
            "range": {
                "type": "noEnd",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2022-03-02",
                "endDate": null
            }
        },
        "applyActions": []
    },
    "additionalNotificationRecipients": []
}
```

## <a name="step-2-retrieve-instances-of-the-access-review"></a>步骤 2：检索访问评审的实例

每个访问评审实例 *都表示每个重复周期，每个唯一资源* 都在审查中。 在步骤 1 中，仅在范围内定义了用户管理员角色资源。 由于定义了定期访问评审，因此实例的 ID 与步骤 1 中计划定义的 ID 不同。

### <a name="request"></a>请求

在以下请求中，替换 `57457d7c-af59-470c-ae71-aa72c657fe0f` 为在步骤 1 中创建的访问评审的值。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-getinstances"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances
```

### <a name="response"></a>响应

在此响应中，实例对象将结束日期显示为开始日期后三天;此时间段在 **accessReviewScheduleDefinition** 对象的 **instanceDurationInDays** 属性的步骤 1 中定义。 *仅返回一个实例，表示只有一个正在审查的资源的第一次重复。*

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('57457d7c-af59-470c-ae71-aa72c657fe0f')/instances",
    "@odata.count": 1,
    "value": [
        {
            "id": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "startDateTime": "2022-03-02T15:31:14.607Z",
            "endDateTime": "2022-03-05T15:31:14.607Z",
            "status": "InProgress",
            "scope": {
                "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
                "principalScopes": [
                    {
                        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                        "query": "/v1.0/users",
                        "queryType": "MicrosoftGraph",
                        "queryRoot": null
                    },
                    {
                        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                        "query": "/v1.0/groups",
                        "queryType": "MicrosoftGraph",
                        "queryRoot": null
                    }
                ],
                "resourceScopes": [
                    {
                        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                        "query": "/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
                        "queryType": "MicrosoftGraph",
                        "queryRoot": null
                    }
                ]
            },
            "reviewers": [
                {
                    "query": "/v1.0/users/f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
                    "queryType": "MicrosoftGraph",
                    "queryRoot": null
                }
            ],
            "fallbackReviewers": []
        }
    ]
}
```

此访问评审实例的状态为 `InProgress`。 状态 `InProgress` 意味着审阅实例是开放的，审阅者可以提交决策，并且此访问评审实例的期限尚未过期。 你还收到了来自 Microsoft Azure 的电子邮件通知，请求执行访问评审。

## <a name="step-3-retrieve-access-review-decisions-before-recording-any-decisions"></a>步骤 3：在记录任何决策之前检索访问评审决策

在发布决策之前，让我们先检查等待决策的项目。

### <a name="request"></a>请求

在以下请求中，替换以下值：

+ `57457d7c-af59-470c-ae71-aa72c657fe0f` 具有在步骤 1 中创建的访问评审的值。
+ `ad0dd148-5d16-4cfd-86e9-ab502f819aaf` 使用要检索其决策的访问评审实例的值。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-getnodecisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions
```

### <a name="response"></a>响应

以下响应显示两个决策项，每个决策项对应于每个主体对资源的访问权限的决策。

+ 主体属性显示两个主体有权访问“用户管理员”角色-一个名为 **IT Helpdesk (用户)** 的组和一个名为 **Aline Dupuy 的** 用户。
+ 决策`NotReviewed`属性的值指示审阅者尚未审阅并发布其决策。
+ 由于在步骤 1 中的 **accessReviewScheduleDefinition** 中未启用建议，因此没有提供任何建议。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accessReviewInstanceDecisionItem)"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('57457d7c-af59-470c-ae71-aa72c657fe0f')/instances('ad0dd148-5d16-4cfd-86e9-ab502f819aaf')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "4d79fbf6-36e6-430b-ba0a-2a727a480303",
            "accessReviewId": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "NoInfoAvailable",
            "principalLink": "https://graph.microsoft.com/v1.0/users/339143ab-541e-484f-b017-e1707e962d34",
            "resourceLink": "https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "resource": {
                "id": "fe930be7-5e62-47db-91af-98c3a49a38b1",
                "displayName": "User Administrator",
                "type": "directoryRole"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "339143ab-541e-484f-b017-e1707e962d34",
                "displayName": "Aline Dupuy",
                "type": "user",
                "userPrincipalName": "AlineD@Contoso.com",
                "lastUserSignInDateTime": ""
            }
        },
        {
            "id": "62fd1c5b-04b8-4703-9fd7-dce6232c3775",
            "accessReviewId": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "NoInfoAvailable",
            "principalLink": "https://graph.microsoft.com/v1.0/groups/b5260fca-6d64-4d5a-92df-0c482d40bc4d",
            "resourceLink": "https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "resource": {
                "id": "fe930be7-5e62-47db-91af-98c3a49a38b1",
                "displayName": "User Administrator",
                "type": "directoryRole"
            },
            "principal": {
                "id": "b5260fca-6d64-4d5a-92df-0c482d40bc4d",
                "displayName": "IT Helpdesk (User)",
                "type": "group"
            }
        }
    ]
}
```

作为审阅者，现在可以提交访问评审实例的决策。

## <a name="step-4-record-decisions"></a>步骤 4：记录决策

现在，你将记录访问评审的决策。

公司策略要求仅向组而不是单个用户授予对特权角色的访问权限。 根据公司策略，在批准组的访问权限时，将拒绝 Aline Dupuy 访问权限。

在以下请求中，替换以下值：

+ `57457d7c-af59-470c-ae71-aa72c657fe0f` 具有在步骤 1 中创建的访问评审的值
+ `ad0dd148-5d16-4cfd-86e9-ab502f819aaf` 使用要检索其决策的访问评审实例的值
+ `4d79fbf6-36e6-430b-ba0a-2a727a480303` 访问评审实例的值限于 Aline 的访问权限
+ `62fd1c5b-04b8-4703-9fd7-dce6232c3775` 访问评审实例的值限于 IT 帮助人员组的访问权限

### <a name="approve-the-security-groups-role-assignment"></a>批准安全组的角色分配

#### <a name="request"></a>请求

在以下请求中，你将批准 IT 帮助人员组的访问权限。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-decisionsforgroup"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions/62fd1c5b-04b8-4703-9fd7-dce6232c3775
Content-type: application/json

{
    "decision": "Approve",
    "justification": "The IT Helpdesk requires continued access to the User Administrator role to manage user account support requests, lifecycle, and access to resources"
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```
HTTP/1.1 204 No Content
```

### <a name="deny-the-individual-user-their-role-assignment"></a>拒绝单个用户的角色分配

#### <a name="request"></a>请求

在以下请求中，将拒绝 Aline Dupuy 的访问权限。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-decisionsforuser"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions/4d79fbf6-36e6-430b-ba0a-2a727a480303
Content-type: application/json

{
    "decision": "Deny",
    "justification": "Aline Dupuy should join an allowed group to maintain access to the User Administrator role. For more details, refer to the company policy '#132487: Privileged roles'"
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```
HTTP/1.1 204 No Content
```

检索访问评审决策 (重复步骤 3) 时，它们具有以下设置：
+ IT 帮助人员组的访问评审决定是在 `Approve` Aline `Deny`的时候作出的。
+ reviewBy 对象包含以审阅者身份的详细信息。
+ applyResult 表示 `New` 尚未应用决策。

虽然你已记录此实例的所有挂起的决策，但尚未将决策应用于资源和主体对象。 例如，Aline 仍然有权访问特权角色。 可以通过运行以下查询 `https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq 'fe930be7-5e62-47db-91af-98c3a49a38b1'`来验证此分配。 此行为是因为 **autoApplyDecisionsEnabled** 已设置为 `false`，你尚未停止审阅，并且实例期尚未结束。

在本教程中，不会手动停止实例，但会让实例自动结束，然后应用决策。

> [!TIP]
>
> 1. 在访问评审实例的 **状态** 标记为 `Completed`之前，仍可更改决策。 重新运行步骤 4，为主体应用不同的决策。
> 2. 还可以手动停止访问评审实例，以便加快步骤 5 的进度。

## <a name="step-5-apply-access-review-decisions"></a>步骤 5：应用访问评审决策

作为管理员，在访问评审实例的 **状态** 设置为 `Completed`后，可以应用决策。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-applydecisions"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/applyDecisions
```

### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```
HTTP/1.1 204 No Content
```

Aline 现在已失去对“用户管理员”角色的访问权限，而 IT 帮助人员组已保留其访问权限。 可以通过运行以下查询 `https://graph.microsoft.com/v1.0/roleManagement/directory/roleAssignments?$filter=roleDefinitionId eq 'fe930be7-5e62-47db-91af-98c3a49a38b1'`来验证角色分配的此状态。

应用决策后，访问评审实例的 **状态** 将为 `Applied`。 此外，由于我们在步骤 1 中创建了定期访问评审，因此将启动一个新实例。 其开始日期为三个月后，当前审阅期标记为已结束。

## <a name="step-6-retrieve-access-review-decisions"></a>步骤 6：检索访问评审决策

Contoso 的审核员正在审查授予或拒绝访问组织中特权角色的所有决定。 你将检索所有限于特权角色的访问评审决策日志。 在此示例中，你将检索在步骤 1 中创建 **的 accessReviewScheduleDefinition** 的决策日志。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-getdecisions"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/ad0dd148-5d16-4cfd-86e9-ab502f819aaf/decisions
```

### <a name="response"></a>响应

以下响应对象不同于在步骤 3 中收到的具有以下设置的响应对象：
+ IT 帮助人员的访问评审 **决定** 是在 `Approve` Aline `Deny`的时候作出的。
+ **reviewBy** 对象包含作为审阅者的基本详细信息。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.accessReviewInstanceDecisionItem)"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('57457d7c-af59-470c-ae71-aa72c657fe0f')/instances('ad0dd148-5d16-4cfd-86e9-ab502f819aaf')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "4d79fbf6-36e6-430b-ba0a-2a727a480303",
            "accessReviewId": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "reviewedDateTime": "2022-03-02T16:50:21.227Z",
            "decision": "Deny",
            "justification": "Aline Dupuy should join an allowed group to maintain access to the User Administrator role. For more details, refer to the company policy '#132487: Privileged roles'",
            "appliedDateTime": "2022-03-02T17:21:05.363Z",
            "applyResult": "AppliedSuccessfully",
            "recommendation": "NoInfoAvailable",
            "principalLink": "https://graph.microsoft.com/v1.0/users/339143ab-541e-484f-b017-e1707e962d34",
            "resourceLink": "https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
            "reviewedBy": {
                "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
                "displayName": "Alex Wilber",
                "type": null,
                "userPrincipalName": "AlexW@Contoso.com"
            },
            "appliedBy": {
                "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
                "displayName": "Alex Wilber",
                "type": null,
                "userPrincipalName": "AlexW@Contoso.com"
            },
            "resource": {
                "id": "fe930be7-5e62-47db-91af-98c3a49a38b1",
                "displayName": "User Administrator",
                "type": "directoryRole"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "339143ab-541e-484f-b017-e1707e962d34",
                "displayName": "Aline Dupuy",
                "type": "user",
                "userPrincipalName": "AlineD@Contoso.com",
                "lastUserSignInDateTime": ""
            }
        },
        {
            "id": "62fd1c5b-04b8-4703-9fd7-dce6232c3775",
            "accessReviewId": "ad0dd148-5d16-4cfd-86e9-ab502f819aaf",
            "reviewedDateTime": "2022-03-02T16:31:04.357Z",
            "decision": "Approve",
            "justification": "The IT Helpdesk requires continued access to the User Administrator role to manage user account support requests, lifecycle, and access to resources.",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "NoInfoAvailable",
            "principalLink": "https://graph.microsoft.com/v1.0/groups/b5260fca-6d64-4d5a-92df-0c482d40bc4d",
            "resourceLink": "https://graph.microsoft.com/beta/roleManagement/directory/roleDefinitions/fe930be7-5e62-47db-91af-98c3a49a38b1",
            "reviewedBy": {
                "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
                "displayName": "Alex Wilber",
                "type": null,
                "userPrincipalName": "AlexW@Contoso.com"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "type": null,
                "userPrincipalName": ""
            },
            "resource": {
                "id": "fe930be7-5e62-47db-91af-98c3a49a38b1",
                "displayName": "User Administrator",
                "type": "directoryRole"
            },
            "principal": {
                "id": "b5260fca-6d64-4d5a-92df-0c482d40bc4d",
                "displayName": "IT Helpdesk (User)",
                "type": "group"
            }
        }
    ]
}
```

<!-- comment this out until a bug is fixed

## Step 7: Retrieve access review history definitions

Contoso's auditors also want to review the access review history for the last quarter. In this example, you'll generate an access review history report for all **accessReviewScheduleDefinition** objects scoped to directory role assignments (roleAssignmentScheduleInstances). In this query, the **decisions** property is empty and therefore defaults to include all decisions in the history report.

First, you'll define the scope of the history report. Then, you generate a download URI that the auditors will use to download the report. The download URI is active for only 24 hours. So, after expiry, you can regenerate another download URI from the previously defined history report.

### Define the scope of the access review history data

In the following request, an empty **decisions** object means all decisions related to the scope of the access review will be included in the history report.

#### Request

```http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/historyDefinitions

{
    "displayName": "Last quarter's access reviews for privileged roles - User Administrator",
    "decisions": [],
    "reviewHistoryPeriodStartDateTime": "2022-03-01T00:00:00Z",
    "reviewHistoryPeriodEndDateTime": "9999-12-31T00:00:00Z",
    "scopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "queryType": "MicrosoftGraph",
            "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances')"
        }
    ]
}
```

#### Response

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/historyDefinitions/$entity",
    "id": "983db508-b77b-427d-ab90-a4041efa658d",
    "displayName": "Last quarter's access reviews for privileged roles - User Administrator",
    "reviewHistoryPeriodStartDateTime": "2022-03-01T00:00:00Z",
    "reviewHistoryPeriodEndDateTime": "9999-12-31T00:00:00Z",
    "decisions": [
        "approve",
        "deny",
        "dontKnow",
        "notReviewed",
        "notNotified"
    ],
    "status": "requested",
    "createdDateTime": "2022-03-02T18:08:51.9032457Z",
    "fulfilledDateTime": null,
    "downloadUri": null,
    "createdBy": {
        "id": "f674a1c9-4a40-439c-bfa3-4b61a9f29d85",
        "displayName": "Alex Wilber",
        "type": null,
        "userPrincipalName": "AlexW@Contoso.com"
    },
    "scopes": [
        {
            "@odata.type": "#microsoft.graph.accessReviewQueryScope",
            "query": "/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, 'roleAssignmentScheduleInstances')",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ]
}
```

### Retrieve the instances of the access review history

#### Request

```msgraph-interactive
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/historyDefinitions/983db508-b77b-427d-ab90-a4041efa658d/instances
```

#### Response

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/historyDefinitions('983db508-b77b-427d-ab90-a4041efa658d')/instances",
    "value": [
        {
            "id": "983db508-b77b-427d-ab90-a4041efa658d",
            "reviewHistoryPeriodStartDateTime": "2022-03-01T00:00:00Z",
            "reviewHistoryPeriodEndDateTime": "9999-12-31T00:00:00Z",
            "status": "done",
            "runDateTime": "2022-03-02T18:08:51.9032457Z",
            "fulfilledDateTime": "2022-03-02T18:08:55.8336038Z",
            "downloadUri": null
        }
    ]
}
```

### Generate a link to download the history report from the instance of the access review history

#### Request

```http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/historyDefinitions/57457d7c-af59-470c-ae71-aa72c657fe0f/instances/983db508-b77b-427d-ab90-a4041efa658d/generateDownloadUri()
```

#### Response

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#accessReviewHistoryInstance",
    "@odata.type": "#microsoft.graph.accessReviewHistoryInstance",
    "id": "a222f18d-5cf5-4210-874c-14d0a7d930b3",
    "reviewHistoryPeriodStartDateTime": "2021-01-01T00:00:00Z",
    "reviewHistoryPeriodEndDateTime": "9999-12-31T00:00:00Z",
    "status": "done",
    "runDateTime": "2022-02-22T10:08:08.2057428Z",
    "fulfilledDateTime": "2022-02-22T10:09:28.5862766Z",
    "downloadUri": "https://ermconsolreportweu.blob.core.windows.net/erm-reports/Last quarter's group reviews April 2021-a222f18d-5cf5-4210-874c-14d0a7d930b3.csv?skoid=4ad0868b-7b78-4869-abb7-8f29151d8428&sktid=33e01921-4d64-4f8c-a055-5bdaffd5e33d&skt=2022-02-22T10:11:22Z&ske=2022-02-22T10:13:22Z&sks=b&skv=2020-04-08&sv=2020-04-08&st=2022-02-22T10:11:22Z&se=2022-02-23T10:11:22Z&sr=b&sp=r&sig=5eX5BfVLS58QqF7oguRH8TeSQdXDHZlapY3y1U%2FGz%2BM%3D"
}
```

The downloadUri property contains a link to download the history report in an Excel file format. This link is active for only 24 hours.

-->
## <a name="step-7-clean-up-resources"></a>第 7 步：清理资源

删除为本教程创建的 **accessReviewScheduleDefinition** 对象。 由于访问评审计划定义是访问评审的蓝图，因此删除该定义将删除设置、实例和决策。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-priviegedroles-deleteaccessreview"
}-->
```msgraph-interactive
DELETE https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/57457d7c-af59-470c-ae71-aa72c657fe0f
```

### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="conclusion"></a>结论

你已了解如何在 Azure AD 中查看对特权角色的访问权限。 组织可以使用访问评审 API 来持续管理对其资源的特权访问，包括 Azure AD 角色和 Azure 资源角色。 除了用户和组，还可以查看应用程序和服务主体对特权角色的访问权限。

## <a name="see-also"></a>另请参阅

+ [访问评审 API 参考](/graph/api/resources/accessreviewsv2-root)
+ [使用 Microsoft 图形 API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)
+ [了解特权访问管理](/microsoft-365/compliance/privileged-access-management-overviewe)