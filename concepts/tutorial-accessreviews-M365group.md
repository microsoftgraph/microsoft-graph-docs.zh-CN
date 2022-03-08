---
title: 教程：使用访问评审 API 查看来宾对组Microsoft 365访问
description: 使用访问评审 API 查看来宾对组Microsoft 365访问
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: f2c9210b4173850c6fbccaad352c88b894965e29
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334917"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-guest-access-to-your-microsoft-365-groups"></a>教程：使用访问评审 API 查看来宾对组Microsoft 365访问

Microsoft Graph 中的访问评审 API 使组织能够审核和证明标识 (也称为) 分配给组织中资源的访问权限。 在跨租户协作中，外部用户可以访问文件、笔记、日历等资源，甚至可以访问Teams对话。 可通过组管理此Microsoft 365管理。 因此，使用访问评审 API，组织可以定期向有权访问此类组的主体以及组织中其他资源的主体提供证明。

假设你已授予外部用户的访问权限 (也称为来宾用户) 组访问Microsoft 365资源。 本教程将指导你查看他们对租户中Microsoft 365组的访问权限。

>[!NOTE]
>为了可读性，本教程中显示的响应对象可能会缩短。

## <a name="prerequisites"></a>先决条件

若要完成本教程，需要以下资源和权限：

+ 启用Azure AD EMS E5 Azure AD Premium P2工作租户。 
+ 不同租户Azure AD中的帐户或作为来宾用户邀请的社交标识 (B2B 用户) 。
+ 以用户[Graph](https://developer.microsoft.com/graph/graph-explorer)登录资源管理器全局管理员角色。 
+ 以下委派权限：、`User.Invite.All`、`AccessReview.ReadWrite.All`、`Group.ReadWrite.All``User.ReadWrite.All`。

若要同意在资源管理器中Graph权限：
1. 选择用户帐户详细信息右边的设置图标，然后选择" **选择权限"**。
   
   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="选择&quot;microsoft Graph权限&quot;。" border="true":::

2. 滚动浏览这些权限的权限列表：
   + AccessReview (3) ，展开并选择 **AccessReview.ReadWrite.All**。
   + 将 (2) ，展开，然后选择 **Group.ReadWrite.All**。
   + 用户 (8) ，展开，然后选择 **User.Invite.All** 和 **User.ReadWrite.All**。
   
   选择“**同意**”，然后选择“**接受**”，以接受同意权限。 你无需代表你的组织同意这些权限。
   
   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="同意 Microsoft Graph权限。" border="true":::

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

## <a name="step-2-invite-a-guest-user-into-your-tenant"></a>步骤 2：将来宾用户邀请到租户

使用电子邮件地址邀请来宾用户 **john@tailspintoys.com** 租户。

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

## <a name="step-3-create-a-new-microsoft-365-group-and-add-the-guest-user"></a>步骤 3：创建新的Microsoft 365组并添加来宾用户

在此步骤中：
1. 创建名为"Microsoft 365 **市场营销活动"的新组**。
2. 将自己分配为组所有者。
3. 添加 john@tailspintoys.com 作为组的成员。 他们访问组是由你（组所有者）审查的主题。

### <a name="request"></a>请求

在此调用中，替换：
+ `cdb555e3-b33e-4fd5-a427-17fadacbdfa7` 使用你的 ID。 若要检索 ID，请运行 `GET` 。`https://graph.microsoft.com/v1.0/me`
+ `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` 使用 **john@tailspintoys.com** 2 中响应的 ID。

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

现在，你有一Microsoft 365来宾用户的组。

## <a name="step-4-create-an-access-review-for-all-microsoft-365-groups-with-guest-users"></a>步骤 4：为具有来宾用户的所有Microsoft 365组创建访问评审

为具有来宾用户的所有 Microsoft 365 组创建定期访问评审系列时，安排定期查看来宾对 Microsoft 365 组的访问权限。 在这种情况下，" **感觉良好"市场营销活动** 组。

访问评审系列使用下列设置：
+ 这是定期访问评审，每季度查看一次。
+ 组所有者决定来宾用户是否应该维护其访问权限。
+ 审阅范围仅限于具有来宾 **Microsoft 365组。**
+ 备份审阅者。 它们可以是回退用户或可在组未分配任何所有者的情况下查看访问权限的组。
+ **autoApplyDecisionsEnabled** 设置为 `true`。 在这种情况下，一旦审阅者完成访问评审或访问评审持续时间结束，将自动应用决策。 如果未启用，用户必须在审阅完成后手动应用决策。
+ 将 **removeAccessApplyAction** 操作应用于拒绝的来宾用户，以将其从组中删除。 来宾用户仍可登录到你的租户，但无法访问组。

### <a name="request"></a>请求

在此调用中，替换以下值：

+ `c9a5aff7-9298-4d71-adab-0a222e0a05e4` 具有指定为备份审阅者的 Aline 的 ID。
+ **startDate** 的值（具有今天的日期）和 **endDate** 值（开始日期为一年）。 

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

以下查询列出了访问评审定义的所有实例。 如果租户中具有来宾Microsoft 365多个组，此请求将为具有来宾用户的每个 Microsoft 365 *组返回一个实例*。

### <a name="request"></a>请求

在此调用中，将 替换为 `c22ae540-b89a-4d24-bac0-4ef35e6591ea` 步骤 4 中返回的访问评审定义的 ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-list_accessReviewInstance"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances
```

### <a name="response"></a>响应

在此响应中，`59ab642a-2776-4e32-9b68-9ff7a47b7f6a`范围包括由 (步骤 3 中创建的"感觉良好"市场营销活动组标识的组) 因为它有来宾用户。

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
在此响应中，访问评审实例当前为 `InProgress`。 因为它是每季度评审一次，所以每三个月自动创建一个新的审阅实例，审阅者可以应用新决策。

## <a name="step-6-get-decisions"></a>步骤 6：获取决策

获取针对访问评审实例做出的决策。

### <a name="request"></a>请求

在此调用中：
+ 将 `c22ae540-b89a-4d24-bac0-4ef35e6591ea` 替换为步骤 4 中返回的访问评审定义的 ID。
+ 将 `6392b1a7-9c25-4844-83e5-34e23c88e16a` 替换为步骤 5 中返回的访问评审实例的 ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-M365group-list_accessReviewInstanceDecisionItem"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances/6392b1a7-9c25-4844-83e5-34e23c88e16a/decisions
```

### <a name="response"></a>响应

以下响应显示为评价实例做出的决定。

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

在如下所示的季度评审中，只要访问评审仍处于活动状态：
+ 每三个月将创建一个新的审阅实例。
+ 审阅者需要为新实例应用新决策。


## <a name="step-7-clean-up-resources"></a>第 7 步：清理资源

删除为本教程创建的资源-**"感觉良好** "市场营销活动组、访问评审计划定义、来宾用户和测试用户。

### <a name="delete-the-microsoft-365-group"></a>删除Microsoft 365组

#### <a name="request"></a>请求

在此调用中，将 替换为`59ab642a-2776-4e32-9b68-9ff7a47b7f6a`"感觉良好"市场营销 **活动组** Microsoft 365 ID。

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

在此调用中，将 替换为 `c22ae540-b89a-4d24-bac0-4ef35e6591ea` 访问评审定义的 ID。 由于访问评审计划定义是访问评审的蓝图，删除该定义将删除相关设置、实例和决策。

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

在此调用中，将 替换为 `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` 来宾用户的 ID，john@tailspintoys.com。

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
在此调用中，将 `c9a5aff7-9298-4d71-adab-0a222e0a05e4` 替换为测试用户的 ID。

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

恭喜！ 你已针对租户中 Microsoft 365 中的来宾用户创建了访问评审，并计划每季度进行一次。 组所有者将在这些周期内查看访问权限，选择批准或拒绝访问。

## <a name="see-also"></a>另请参阅


+ [访问评审 API](/graph/api/resources/accessreviewsv2-overview)
+ [访问Azure AD是什么？](/azure/active-directory/governance/access-reviews-overview)
+ [在访问评审中查看Azure AD和应用程序的访问权限](/azure/active-directory/governance/perform-access-review)