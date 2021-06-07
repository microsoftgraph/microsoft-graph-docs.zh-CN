---
title: 教程：使用访问评审 API 查看来宾对组Microsoft 365访问
description: 使用访问评审 API 查看来宾对组Microsoft 365访问
author: FaithOmbongi
localization_priority: Normal
ms.prod: governance
ms.openlocfilehash: ad34932926a658d498242dd168ac7fee1d2b31a1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751137"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-guest-access-to-your-microsoft-365-groups"></a>教程：使用访问评审 API 查看来宾对组Microsoft 365访问

在本教程中，你将使用 Graph 资源管理器创建和阅读访问评审，这些评论面向租户Microsoft 365来宾用户的所有组。 若要实现此目的，你将首先使用 Azure AD B2B 邀请并创建租户中的来宾用户（也称为外部标识）。 然后，在创建和阅读访问评审之前，Microsoft 365此来宾用户添加到你的组。

>[!NOTE]
>为了可读性，本教程中显示的响应对象可能会缩短。

## <a name="prerequisites"></a>先决条件

若要完成本教程，需要以下资源和权限：

+ 启用 Azure AD 或 EMS E5 许可证高级版 Azure AD 租户。 
+ 不同 Azure AD 租户中的帐户或作为来宾用户邀请的社交标识 (B2B) 。
+ 以用户[Graph](https://developer.microsoft.com/graph/graph-explorer)用户登录浏览器全局管理员角色。 
+ 以下委派权限 `User.Invite.All` `AccessReview.ReadWrite.All` ：、、、。 `Group.ReadWrite.All` `User.ReadWrite.All`

若要同意在浏览器浏览器中Graph权限：
1. 选择用户帐户详细信息右侧设置图标，然后选择"**选择权限"。**
   
   ![选择 Microsoft Graph 权限](../images/../concepts/images/tutorial-accessreviews-api/settings.png)
   <!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="Select the Microsoft Graph permissions":::-->

2. 滚动浏览这些权限的权限列表：
   + AccessReviews (3) ，展开，然后选择 **AccessReviews.ReadWrite.All**。
   + 将 (2) ，展开，然后选择 **Group.ReadWrite.All。**
   + 用户 (8) ，展开，然后选择 **User.Invite.All** 和 **User.ReadWrite.All。**
   
   选择“**同意**”，然后选择“**接受**”，以接受同意权限。 你不需要代表组织同意这些权限。
   
   ![同意 Microsoft Graph权限](../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png)
   <!--:::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions_M365.png" alt-text="Consent to the Microsoft Graph permissions":::-->

## <a name="step-1-create-a-test-user-in-your-tenant"></a>步骤 1：在租户中创建测试用户

### <a name="request"></a>请求

```http
POST /users
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

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#users/$entity",
    "id": "c9a5aff7-9298-4d71-adab-0a222e0a05e4",
    "displayName": "Aline Dupuy",
    "userPrincipalName": "AlineD@contoso.com",
    "userType": "Member"
}
```

## <a name="step-2-invite-a-guest-user-into-your-tenant"></a>步骤 2：将来宾用户邀请到租户

使用电子邮件地址邀请来宾用户 **john@tailspintoys.com** 租户。

### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/beta/invitations
Content-Type: application/json

{
    "invitedUserDisplayName": "John Doe (Tailspin Toys)",
    "invitedUserEmailAddress": "john@tailspintoys.com",
    "sendInvitationMessage": false,
    "inviteRedirectUrl": "https://myapps.microsoft.com"
}
```

### <a name="response"></a>响应

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#invitations/$entity",
    "invitedUser": {
        "id": "baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    }    
}
```

## <a name="step-3-create-a-new-microsoft-365-group-and-add-the-guest-user"></a>步骤 3：新建Microsoft 365组并添加来宾用户

在此步骤中：
1. 创建一个名为"Microsoft 365 **市场营销活动"的新组**。
2. 将自己分配为组所有者。
3. 添加 john@tailspintoys.com 作为组成员。 他们访问组是由你（组所有者）审查的主题。

### <a name="request"></a>请求
在此调用中，替换：
+ `cdb555e3-b33e-4fd5-a427-17fadacbdfa7` 与 **id 一起**。若要检索 **id，** 请运行 `GET` `https://graph.microsoft.com/beta/me` 。
+ `baf1b0a0-1f9a-4a56-9884-6a30824f8d20`john@tailspintoys.com 步骤 2 **中响应** 的 id。

```http
POST https://graph.microsoft.com/beta/groups
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
        "https://graph.microsoft.com/beta/users/cdb555e3-b33e-4fd5-a427-17fadacbdfa7"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20"
    ]
}
```

### <a name="response"></a>响应

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#groups/$entity",
    "id": "59ab642a-2776-4e32-9b68-9ff7a47b7f6a",
    "displayName": "Feelgood Marketing Campaign",
    "groupTypes": [
        "Unified"
    ]
}
```

现在，你有一Microsoft 365来宾用户的组。

## <a name="step-4-create-an-access-review-for-all-microsoft-365-groups-with-guest-users"></a>步骤 4：为具有来宾用户的所有Microsoft 365组创建访问评审

为具有来宾用户的所有 Microsoft 365 组创建定期访问评审系列时，安排定期查看来宾对 Microsoft 365 组的访问权限。 为 **"Feelgood 市场营销活动"组** 进行此操作。

访问评审系列使用下列设置：
+ 这是定期访问评审，每季度查看一次。
+ 组所有者查看来宾用户的持续访问权限。
+ 审查范围仅限于仅限Microsoft 365 **来宾用户的组**。 有关配置范围的更多选项，请参阅另 [请参阅部分](#see-also) 。 
+ 备份审阅者。 这可以是回退用户或可在组未分配任何所有者的情况下查看访问权限的组。 有关配置审阅者的更多选项，请参阅另 [请参阅部分](#see-also) 。
+ **autoApplyDecisionsEnabled** 设置为 `true` 。 在这种情况下，一旦审阅者完成访问评审或访问评审持续时间结束，将自动应用决策。 如果未启用，则用户必须在审阅完成后手动应用决策。
+ 将 **removeAccessApplyAction** 操作应用于拒绝的来宾用户。 这将删除被拒绝来宾组的成员身份。 来宾用户仍可登录到你的租户。

### <a name="request"></a>请求
在此调用中，替换以下内容：

+ `c9a5aff7-9298-4d71-adab-0a222e0a05e4` 使用 **要** 指定为备份审阅者的用户的 ID。 这是步骤 1 中响应的 **ID。**
+ **startDate** 的值，其当前日期和 **endDate** 值，其日期为从开始日期起一年。 

```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
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
    "backupReviewers": [
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

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
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
    "backupReviewers": [
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

以下查询列出了访问评审定义的所有实例。 如果测试租户包含Microsoft 365用户的其他组，此请求将为租户中具有来宾Microsoft 365组返回一个实例。

### <a name="request"></a>请求
在此调用中， `c22ae540-b89a-4d24-bac0-4ef35e6591ea` 将 替换为步骤 4 中返回的访问评审定义的 ID。

```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances
```

### <a name="response"></a>响应
在此响应中，范围包括一个 **id** 为 (在步骤 3 中创建的 Feelgood 市场营销活动组) `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` 因为它有来宾用户。 

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances",
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
在此响应中，访问评审实例当前为 `InProgress` 。 因为这是每季度评审一次，每 3 个月将自动创建一个新的审阅实例，并且审阅者可以应用新决策。

## <a name="step-6-get-decisions"></a>步骤 6：获取决策

获取针对访问评审实例做出的决策。

### <a name="request"></a>请求
在此调用中：
+ 将 `c22ae540-b89a-4d24-bac0-4ef35e6591ea` 替换为步骤 4 中返回的访问评审定义的 ID。
+ 将 `6392b1a7-9c25-4844-83e5-34e23c88e16a` 替换为步骤 5 中返回的访问评审实例的 ID。

```http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea/instances/6392b1a7-9c25-4844-83e5-34e23c88e16a/decisions
```

### <a name="response"></a>响应

以下响应显示为评价实例做出的决定。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('c22ae540-b89a-4d24-bac0-4ef35e6591ea')/instances('6392b1a7-9c25-4844-83e5-34e23c88e16a')/decisions",
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

因为这是季度评审，并且只要定义仍处于活动状态（即重复的 **endDate** 不是过去日期，每 3 个月创建一次新的审阅实例，您作为审阅者就可以应用新决策。

## <a name="step-7-clean-up-resources"></a>第 7 步：清理资源

删除为本教程创建的资源- 体验市场营销活动组、访问 **评审** 计划定义、来宾用户和测试用户。

### <a name="delete-the-microsoft-365-group"></a>删除Microsoft 365组

#### <a name="request"></a>请求
在此调用中， `59ab642a-2776-4e32-9b68-9ff7a47b7f6a` 将 替换为 **你的 Feelgood 市场营销活动的** **id** Microsoft 365组。

```http
DELETE https://graph.microsoft.com/beta/groups/59ab642a-2776-4e32-9b68-9ff7a47b7f6a
```

#### <a name="response"></a>响应

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-access-review-definition"></a>删除访问评审定义

在此调用中， `c22ae540-b89a-4d24-bac0-4ef35e6591ea` 将 替换为 **访问** 评审定义的 ID。 由于访问评审计划定义是访问评审的蓝图，删除该定义将删除与访问评审相关的设置、实例和决策。

#### <a name="request"></a>请求
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/c22ae540-b89a-4d24-bac0-4ef35e6591ea
```

#### <a name="response"></a>响应
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```
### <a name="remove-the-guest-user"></a>删除来宾用户

在此调用中， `baf1b0a0-1f9a-4a56-9884-6a30824f8d20` 将 替换为 **来宾用户的 ID，john@tailspintoys.com。**

#### <a name="request"></a>请求
```http
DELETE https://graph.microsoft.com/beta/users/baf1b0a0-1f9a-4a56-9884-6a30824f8d20
```

#### <a name="response"></a>响应
```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

### <a name="delete-the-test-user"></a>删除测试用户

#### <a name="request"></a>请求
在此调用中， `c9a5aff7-9298-4d71-adab-0a222e0a05e4` 将 替换为 **测试** 用户的 ID。

```http
DELETE https://graph.microsoft.com/beta/users/c9a5aff7-9298-4d71-adab-0a222e0a05e4
```

#### <a name="response"></a>响应

```http
HTTP/1.1 204 No Content
Content-type: text/plain
```

恭喜！ 你已针对租户中 Microsoft 365 组的所有来宾用户创建了访问评审，并计划每季度评估并证明来宾用户的访问权限。 组所有者将在这些周期内查看访问权限，选择批准或拒绝访问。

## <a name="see-also"></a>另请参阅

+ [访问评审 API 参考](/graph/api/resources/accessreviewsv2-root?view=graph-rest-beta&preserve-view=true)
+ [使用 Microsoft Graph API 配置访问评审定义的范围](/graph/accessreviews-scope-concept)
+ [使用 Microsoft Graph API 将审阅者分配给你的访问Graph定义](/graph/accessreviews-reviewers-concept)
+ [访问评审概述和许可证要求](/azure/active-directory/governance/access-reviews-overview)
+ [创建对应用程序应用程序的组&评审](/azure/active-directory/governance/create-access-review)
+ [邀请/添加来宾用户到组织](/graph/api/resources/invitation?view=graph-rest-beta&preserve-view=true)

