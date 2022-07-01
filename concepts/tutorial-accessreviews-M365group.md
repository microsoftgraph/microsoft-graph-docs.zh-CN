---
title: 教程：使用访问评审 API 查看来宾对 Microsoft 365 组的访问权限
description: 了解如何使用访问评审 API 通过 Azure AD 租户中的 Microsoft 365 组查看外部/来宾用户对组织资源的访问权限。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 972a3cb1aa8618370cf78d5921d16a699dd6b0b8
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437560"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-guest-access-to-your-microsoft-365-groups"></a>教程：使用访问评审 API 查看来宾对 Microsoft 365 组的访问权限

Microsoft Graph 中的访问评审 API 使组织能够审核和证明标识 (也称为 *主体*) 分配给组织中资源的访问权限。 在跨租户协作中，外部用户可以访问文件、笔记、日历甚至 Teams 对话等资源。 可以通过 Microsoft 365 组有效地管理此访问。 因此，使用访问评审 API，组织可以定期证明有权访问此类组的主体以及组织中的其他资源。

假设你已向外部用户授予访问权限， (也通过 Microsoft 365 组向组织中的资源) 来 *宾用户* 。 本教程将指导你查看他们对租户中 Microsoft 365 组的访问权限。

>[!NOTE]
>本教程中显示的响应对象可能会缩短以实现可读性。

## <a name="prerequisites"></a>先决条件

若要完成本教程，需要以下资源和权限：

+ 已启用Azure AD Premium P2或 EMS E5 许可证的工作 Azure AD 租户。 
+ 另一个 Azure AD 租户中的帐户或社交标识，可以邀请其作为来宾用户 (B2B 用户) 。
+ 以全局管理员角色中的用户身份登录 [到 Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer) 。 
+ 以下委派权限： `User.Invite.All`， ， `AccessReview.ReadWrite.All``Group.ReadWrite.All`， . `User.ReadWrite.All`

若要在 Graph 资源管理器中同意所需权限，请执行以下操作：
1. 选择用户帐户详细信息右侧的设置图标，然后选择 **“选择权限**”。
   
   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="选择 Microsoft Graph 权限。" border="true":::

2. 滚动浏览这些权限的权限列表：
   + AccessReview (3) ，展开并选择 **AccessReview.ReadWrite.All**。
   + 组 (2) ，展开，然后选择 **Group.ReadWrite.All**。
   + 用户 (8) ，展开并选择 **User.Invite.All** 和 **User.ReadWrite.All**。
   
   选择“**同意**”，然后选择“**接受**”，以接受同意权限。 无需代表组织同意这些权限。
   
   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="同意 Microsoft Graph 权限。" border="true":::

## <a name="step-1-create-a-test-user-in-your-tenant"></a>步骤 1：在租户中创建测试用户

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-createUser"
}-->

```http
POST https://graph.microsoft.com/v1.0/users
Content-Type: application/json

{
    "accountEnabled": true,
    "displayName": "Aline Dupuy",
    "mailNickname": "AlineD",
    "userPrincipalName": "AlineD@contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": true,
        "password": "xWwvJ]6NMw+bWH-d"
    }
}
```

### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.user"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
    "id": "c9a5aff7-9298-4d71-adab-0a222e0a05e4",
    "displayName": "Aline Dupuy",
    "userPrincipalName": "AlineD@contoso.com",
    "userType": "Member"
}
```

## <a name="step-2-invite-a-guest-user-into-your-tenant"></a>步骤 2：邀请来宾用户进入租户

邀请具有电子邮件地址的来宾用户 **john@tailspintoys.com** 租户。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-inviteguest"
}-->

```http
POST https://graph.microsoft.com/v1.0/invitations
Content-Type: application/json

{
    "invitedUserDisplayName": "John Doe (Tailspin Toys)",
    "invitedUserEmailAddress": "john@tailspintoys.com",
    "sendInvitationMessage": false,
    "inviteRedirectUrl": "https://myapps.microsoft.com"
}
```

### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitation"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#invitations/$entity",
    "invitedUser": {
        "id": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    }    
}
```

## <a name="step-3-create-a-new-microsoft-365-group-and-add-the-guest-user"></a>步骤 3：创建新的 Microsoft 365 组并添加来宾用户

在此步骤中：
1. 创建名为 **“感觉良好的营销活动**”的新 Microsoft 365 组。
2. 将自己分配为组所有者。
3. 将 john@tailspintoys.com 添加为组成员。 他们对组的访问权限由你（组所有者）审阅。

### <a name="request"></a>请求

在此调用中，替换：
+ `cdb555e3-b33e-4fd5-a427-17fadacbdfa7` 使用 ID。 若要检索 ID，请继续`https://graph.microsoft.com/v1.0/me`运行`GET`。
+ `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` 包含 **步骤** 2 中响应的 john@tailspintoys.com ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-creategroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
    "description": "Feelgood Marketing Campaign with external partners and vendors.",
    "displayName": "Feelgood Marketing Campaign",
    "groupTypes": [
        "Unified"
    ],
    "mailEnabled": true,
    "mailNickname": "FeelGoodCampaign",
    "securityEnabled": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/v1.0/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/v1.0/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    ]
}
```

### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group",
  "name": "create_group"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "59ab642a-2776-4e32-9b68-9ff7a47b7f6a",
    "displayName": "Feelgood Marketing Campaign",
    "groupTypes": [
        "Unified"
    ]
}
```

你现在有一个具有来宾用户的 Microsoft 365 组。

## <a name="step-4-create-an-access-review-for-all-microsoft-365-groups-with-guest-users"></a>步骤 4：使用来宾用户为所有 Microsoft 365 组创建访问评审

为所有具有来宾用户的 Microsoft 365 组创建定期访问评审系列时，请定期查看来宾对 Microsoft 365 组的访问权限。 在这种情况下， **感觉良好的市场营销活动** 组。

访问评审系列使用以下设置：
+ 这是定期访问评审，每季度审查一次。
+ 组所有者决定来宾用户是否应保留其访问权限。
+ 评审范围仅限于具有 **来宾用户** 的 Microsoft 365 组。
+ 备份审阅者。 它们可以是回退用户，也可以是可在组未分配任何所有者的情况下查看访问权限的组。
+ **autoApplyDecisionsEnabled** 设置为 `true`。 在这种情况下，一旦审阅者完成访问评审或访问评审持续时间结束，就会自动应用决策。 如果未启用，则用户必须在评审完成后手动应用决策。
+ 对被拒绝的来宾用户应用 **removeAccessApplyAction** 操作，以将其从组中删除。 来宾用户仍然可以登录到租户，但不会访问该组。

### <a name="request"></a>请求

在此调用中，替换以下值：

+ `c9a5aff7-9298-4d71-adab-0a222e0a05e4` 包含要指定为备份审阅者的 Aline ID。
+ **startDate** 的值，其日期和 **endDate** 值为从开始日期起一年的日期。 

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "Group owners review guest across Microsoft 365 groups in the tenant (Quarterly)",
    "descriptionForAdmins": "",
    "descriptionForReviewers": "",
    "scope": {
        "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "./owners",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "fallbackReviewers": [
        {
            "query": "/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Approve",
        "instanceDurationInDays": 0,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
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
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-10",
                "endDate": "2022-12-21"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.removeAccessApplyAction"
            }
        ]
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
    "id": "c22ae540-b89a-4d24-bac0-4ef35e6591ea",
    "displayName": "Group owners review guest across Microsoft 365 groups in the tenant (Quarterly)",
    "status": "NotStarted",
    "createdBy": {
        "id": "cdb555e3-b33e-4fd5-a427-17fadacbdfa7",
        "displayName": "MOD Administrator",
        "userPrincipalName": "admin@contoso.com"
    },
    "scope": {
        "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified'))&$count=true",
        "queryType": "MicrosoftGraph"
    },
    "reviewers": [
        {
            "query": "./owners",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "fallbackReviewers": [
        {
            "query": "/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4",
            "queryType": "MicrosoftGraph",
            "queryRoot": null
        }
    ],
    "settings": {
        "defaultDecisionEnabled": true,
        "defaultDecision": "Approve",
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
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
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2021-02-10",
                "endDate": "2022-12-21"
            }
        },
        "applyActions": [
            {
                "@odata.type": "#microsoft.graph.removeAccessApplyAction"
            }
        ]
    }
}
```

## <a name="step-5-list-instances-of-the-access-review"></a>步骤 5：列出访问评审的实例

以下查询列出了访问评审定义的所有实例。 如果租户中有多个包含来宾用户的 Microsoft 365 组，则此请求将为 *每个包含来宾用户的 Microsoft 365 组返回一个实例*。

### <a name="request"></a>请求

在此调用中，请替换 `c22ae540-b89a-4d24-bac0-4ef35e6591ea` 为步骤 4 中返回的访问评审定义的 ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-list_accessReviewInstance"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances
```

### <a name="response"></a>响应

在此响应中，该范围包括由 (在步骤 3) 中创建 **的“感觉良好”营销活动** 组标识`59ab642a-2776-4e32-9b68-9ff7a47b7f6a`的组，因为它具有来宾用户。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstance",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances",
    "value": [
        {
            "id": "6392b1a7-9c25-4844-83e5-34e23c88e16a",
            "startDateTime": "2021-02-10T17:00:36.96Z",
            "endDateTime": "2021-02-10T17:00:36.96Z",
            "status": "InProgress",
            "scope": {
                "query": "/groups/59ab642a-2776-4e32-9b68-9ff7a47b7f6a/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph"
            }
        }
    ]
}
```
在此响应中，访问评审实例当前 `InProgress`为 。 由于这是季度评审，因此每三个月自动创建一个新的审阅实例，审阅者可以应用新的决策。

## <a name="step-6-get-decisions"></a>步骤 6：获取决策

获取针对访问评审实例做出的决定。

### <a name="request"></a>请求

在此调用中：
+ 替换 `c22ae540-b89a-4d24-bac0-4ef35e6591ea` 为步骤 4 中返回的访问评审定义的 ID。
+ 替换 `6392b1a7-9c25-4844-83e5-34e23c88e16a` 为步骤 5 中返回的访问评审实例的 ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-list_accessReviewInstanceDecisionItem"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances/6392b1a7-9c25-4844-83e5-34e23c88e16a/decisions
```

### <a name="response"></a>响应

以下响应显示为审阅实例做出的决定。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances('6392b1a7-9c25-4844-83e5-34e23c88e16a')/decisions",
    "@odata.count": 1,
    "value": [
        {
            "id": "0e76ee07-b4c6-469e-bc9d-e73fc9a8d660",
            "accessReviewId": "6392b1a7-9c25-4844-83e5-34e23c88e16a",
            "reviewedDateTime": "2021-02-10T17:06:26.147Z",
            "decision": "Approve",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "AAD Access Reviews",
                "userPrincipalName": "AAD Access Reviews"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20",
                "userDisplayName": "John Doe (Tailspin Toys)",
                "userPrincipalName": "john@tailspintoys.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20",
                "displayName": "John Doe (Tailspin Toys)",
                "userPrincipalName": "john@tailspintoys.com"
            }
        }
    ]
}
```

在这样的季度评审中，只要访问评审仍处于活动状态，
+ 每三个月创建一个新的审阅实例。
+ 需要审阅者为新实例应用新决策。


## <a name="step-7-clean-up-resources"></a>第 7 步：清理资源

删除为本教程创建的资源 — **感觉市场营销活动组良好** 、访问评审计划定义、来宾用户和测试用户。

### <a name="delete-the-microsoft-365-group"></a>删除 Microsoft 365 组

#### <a name="request"></a>请求

在此调用中，请替换 `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` 为 **“感觉良好”营销活动** Microsoft 365 组的 ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/59ab642a-2776-4e32-9b68-9ff7a47b7f6a
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-access-review-definition"></a>删除访问评审定义

在此调用中，请替换 `c22ae540-b89a-4d24-bac0-4ef35e6591ea` 为访问评审定义的 ID。 由于访问评审计划定义是访问评审的蓝图，因此删除该定义将删除相关的设置、实例和决策。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="remove-the-guest-user"></a>删除来宾用户

在此调用中，请替换 `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` 为来宾用户的 ID，john@tailspintoys.com。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_user"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-test-user"></a>删除测试用户
在此调用中，请替换 `c9a5aff7-9298-4d71-adab-0a222e0a05e4` 为测试用户的 ID。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-delete_guestuser"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

恭喜！ 你已为租户中的 Microsoft 365 组中的来宾用户创建了访问评审，并按季度计划。 组所有者会在这些周期中查看访问权限，选择批准或拒绝访问权限。

## <a name="see-also"></a>另请参阅


+ [访问评审 API](/graph/api/resources/accessreviewsv2-overview)
+ [什么是 Azure AD 访问评审？](/azure/active-directory/governance/access-reviews-overview)
+ [在 Azure AD 访问评审中查看对组和应用程序的访问权限](/azure/active-directory/governance/perform-access-review)