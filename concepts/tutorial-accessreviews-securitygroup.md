---
title: 教程：使用访问评审 API 查看对安全组的访问权限
description: 了解如何使用访问评审 API 查看对 Azure AD 租户中安全组的访问权限，并在将 API 调用自动执行到脚本或应用之前测试 API 调用。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: 7f64afebad0057b305aa5c3dc2544753aad8d25f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66443807"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-access-to-your-security-groups"></a>教程：使用访问评审 API 查看对安全组的访问权限

Microsoft Graph 中的访问评审 API 使组织能够审核和证明标识 (也称为 *主体*) 分配给组织中资源的访问权限。 管理主体对其他资源的访问权限的最有效方法之一是通过 Azure AD 安全组。 例如，可以将数百个用户分配给安全组，并分配安全组对文件夹的访问权限。 使用访问评审 API，组织可以定期证明有权访问此类组的主体以及组织中的其他资源。

假设使用 Azure AD 安全组分配标识 (也称为 *主体* ，) 访问组织中的资源。 需要定期证明安全组的所有成员都需要其成员身份，并扩展其对分配给安全组的资源的访问权限。

本教程指导你使用访问评审 API 查看对 Azure AD 租户中安全组的访问权限。 在将访问评审 API 调用自动化到脚本或应用之前，可以使用 Graph 资源管理器或 Postman 来试用和测试访问评审 API 调用。 此测试环境可帮助你正确定义和验证查询，而无需反复重新编译应用程序，从而节省时间。

## <a name="prerequisites"></a>先决条件

若要完成本教程，需要以下资源和权限：

+ 已启用Azure AD Premium P2或 EMS E5 许可证的工作 Azure AD 租户。
+ 以全局管理员或标识治理管理员 Azure AD 角色中的用户身份登录 [到 Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) 。
  + [可选]打开新的 **隐身**、 **匿名** 或 **InPrivate 浏览器** 窗口。 本教程稍后将登录。
+ 以下委派权限： `AccessReview.ReadWrite.All`， . `Group.ReadWrite.All`

若要在 Graph 资源管理器中同意所需权限，请执行以下操作：
1. 选择用户帐户详细信息右侧的设置齿轮图标，然后选择 **“选择权限**”。

    :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="选择 Microsoft Graph 权限。" border="true":::

2. 滚动浏览这些权限的权限列表：
   + AccessReview (3) ，展开并选择 **AccessReview.ReadWrite.All**。
   + 组 (2) ，展开，然后选择 **Group.ReadWrite.All**。
  
    选择 **“同意**”，然后在弹出窗口中 **，代表你的组织选择“同意** ”，然后选择“ **接受** ”以接受权限的同意。

   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="同意 Microsoft Graph 权限。" border="true":::
   
>[!NOTE]
>本教程中显示的响应对象可能会缩短以实现可读性。
   
## <a name="step-1-create-test-users-in-your-tenant"></a>步骤 1：在租户中创建测试用户

通过运行以下三次请求创建三个新的测试用户，每次更改 **displayName**、 **mailNickname** 和 **userPrincipalName 属性的** 值。 记录三个新测试用户的 ID。

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-createUser"
}-->
```http
POST https://graph.microsoft.com/v1.0/users
Content-Type: application/json

{
    "accountEnabled": true,
    "displayName": "Adele Vance",
    "mailNickname": "AdeleV",
    "userPrincipalName": "AdeleV@Contoso.com",
    "passwordProfile": {
        "forceChangePasswordNextSignIn": true,
        "password": "xWwvJ]6NMw+bWH-d"
    }
}
```

### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
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
    "id": "3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
    "displayName": "Adele Vance",
    "userPrincipalName": "AdeleV@Contoso.com"
}
```

## <a name="step-2-create-a-security-group-assign-owners-and-add-members"></a>步骤 2：创建安全组、分配所有者和添加成员

创建一个名为 **“生成安全** 性”的安全组，该安全组是本教程中访问评审的目标。 分配给此组一个组所有者和两个成员。

### <a name="request"></a>请求

从上一步开始，你创建了三个测试用户。 其中一个用户将是组所有者，而另外两个用户将是组成员。

在此调用中，替换：
+ `d3bcdff4-4f80-4418-a65e-7bf3778c5dca` 具有组所有者的 ID。
+ `3b8ceebc-49e6-4e0c-9e14-c906374a7ef6` 以及 `bf59c5ba-5304-4c9b-9192-e5a4cb8444e7` 两个组成员的 ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-creategroup"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups
Content-Type: application/json

{
    "description": "Building security",
    "displayName": "Building security",
    "groupTypes": [],
    "mailEnabled": false,
    "mailNickname": "buildingsecurity",
    "securityEnabled": true,
    "owners@odata.bind": [
        "https://graph.microsoft.com/beta/users/d3bcdff4-4f80-4418-a65e-7bf3778c5dca"
    ],
    "members@odata.bind": [
        "https://graph.microsoft.com/beta/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
        "https://graph.microsoft.com/beta/users/bf59c5ba-5304-4c9b-9192-e5a4cb8444e7"
    ]
}
```

### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.group"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#groups/$entity",
    "id": "eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
    "description": "Building security",
    "displayName": "Building security",
    "mailNickname": "buildingsecurity",
    "securityEnabled": true
}
```

从响应中，记录新组的 ID，以便在本教程的后面部分使用它。

## <a name="step-3-create-an-access-review-for-the-security-group"></a>步骤 3：为安全组创建访问评审

### <a name="request"></a>请求

在此调用中，替换以下值：
+ `eb75ccd2-59ef-48b7-8f76-cc3f33f899f4` 具有 **生成安全** 组的 ID。 范围指定将评审应用于 **生成安全** 组的所有成员。 有关配置范围的更多选项，请 [参阅“另请参阅](#see-also) ”部分。
+ **startDate** 值，其日期和 **endDate** 值为从开始日期起的 5 天。

访问评审具有以下设置：

+ 如果未为 **审阅者** 属性指定值，则会推断为自审。 因此，每个组成员都会自我证明其维护对组的访问权限的需要。
+ 评审范围是 **(建筑安全** 组的直接和间接) 的成员。
+ 审阅者必须提供理由来说明为何需要维护对组的访问权限。
+ 默认决策是在 `Deny` 实例过期之前审阅者不响应访问评审请求时作出的。 该 `Deny` 决定将组成员从组中删除。
+ 这是一次性访问评审，五天后结束。 因此，授予访问权限后，用户无需在访问评审期内再次自我证明。
+ 在评审范围内定义的主体将收到电子邮件通知和提醒，提示他们自我证明其维护访问权限的需要。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions
Content-type: application/json

{
    "displayName": "One-time self-review for members of Building security",
    "descriptionForAdmins": "One-time self-review for members of Building security",
    "descriptionForReviewers": "One-time self-review for members of Building security",
    "scope": {
        "query": "/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4/transitiveMembers",
        "queryType": "MicrosoftGraph"
    },
    "instanceEnumerationScope": {
        "query": "/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
        "queryType": "MicrosoftGraph"
    },
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 5,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2022-02-11",
                "endDate": "2022-02-16"
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
    "id": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
    "displayName": "One-time self-review for members of Building security",
    "createdDateTime": null,
    "lastModifiedDateTime": null,
    "status": "NotStarted",
    "descriptionForAdmins": "One-time self-review for members of Building security",
    "descriptionForReviewers": "One-time self-review for members of Building security",
    "createdBy": {
        "id": "bf59c5ba-5304-4c9b-9192-e5a4cb8444e7",
        "displayName": "MOD Administrator",
        "type": null,
        "userPrincipalName": "admin@Contoso.com"
    },
    "scope": {},
    "instanceEnumerationScope": {},
    "reviewers": [],
    "fallbackReviewers": [],
    "settings": {
        "mailNotificationsEnabled": true,
        "reminderNotificationsEnabled": true,
        "justificationRequiredOnApproval": true,
        "defaultDecisionEnabled": true,
        "defaultDecision": "Deny",
        "instanceDurationInDays": 5,
        "autoApplyDecisionsEnabled": true,
        "recommendationsEnabled": true,
        "recurrence": {
            "pattern": null,
            "range": {
                "type": "numbered",
                "numberOfOccurrences": 0,
                "recurrenceTimeZone": null,
                "startDate": "2022-02-11",
                "endDate": "2022-02-16"
            }
        },
        "applyActions": []
    },
    "additionalNotificationRecipients": []
}
```

上述访问评审的状态标记为 **NotStarted**。 可以检索访问评审 (GET `https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b`) 以监视状态，当状态标记为 **InProgress** 时，会为访问评审创建实例，并且可以发布决策。 还可以检索访问评审，查看访问评审的完整设置。

## <a name="step-4-list-instances-of-the-access-review"></a>步骤 4：列出访问评审的实例

将访问评审的 **状态** 标记为 `InProgress`后，运行以下查询以列出访问评审定义的所有实例。 由于在步骤 3 中创建了一次性访问评审，因此请求仅返回一个 ID（如计划定义 ID）的实例。

### <a name="request"></a>请求

在此调用中，请替换 `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` 为步骤 3 中返回的访问评审定义的 ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_accessReviewInstance"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances
```

### <a name="response"></a>响应

在此响应中，实例的 **状态** 是因为 `InProgress` **startDateTime** 已过期， **且 endDateTime** 在将来。 如果 **startDateTime** 是将来的，则状态将为 `NotStarted`。 另一方面，如果 **endDateTime** 是过去，则状态将为 `Completed`。

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/instances",
    "value": [
        {
            "id": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
            "startDateTime": "2022-02-11T17:35:25.24Z",
            "endDateTime": "2022-02-16T08:00:00Z",
            "status": "InProgress",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4/transitiveMembers/microsoft.graph.user",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            },
            "reviewers": [],
            "fallbackReviewers": []
        }
    ]
}
```

## <a name="step-5-who-was-contacted-for-the-review"></a>步骤 5：已联系谁进行评审？

可以确认已联系 **生成安全** 组的所有成员，以发布其针对此访问评审实例的评审决定。

### <a name="request"></a>请求

在此调用中，请替换 `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` 为访问评审计划定义的 ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_contactedReviewers"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/contactedReviewers
```

### <a name="response"></a>响应

以下响应显示， **建筑安全** 组的两名成员已收到待审通知。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewReviewer",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/instances('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/contactedReviewers",
    "@odata.count": 2,
    "value": [
        {
            "id": "3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
            "displayName": "Adele Vance",
            "userPrincipalName": "AdeleV@Contoso.com",
            "createdDateTime": "2022-02-11T17:35:34.4092545Z"
        },
        {
            "id": "bf59c5ba-5304-4c9b-9192-e5a4cb8444e7",
            "displayName": "Alex Wilber",
            "userPrincipalName": "AlexW@Contoso.com",
            "createdDateTime": "2022-02-11T17:35:34.4092545Z"
        }
    ]
}
```

## <a name="step-6-get-decisions"></a>步骤 6：获取决策

你对为访问评审实例做出的决定感兴趣。

### <a name="request"></a>请求

在此调用中，请替换 `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` 为访问评审计划定义和实例的 ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_accessReviewInstanceDecisionItem"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/decisions
```

### <a name="response"></a>响应

以下响应显示对审阅实例做出的决定。 由于 **生成安全** 性有两个成员，因此需要两个决策项。

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identityGovernance/accessReviews/definitions('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/instances('2d56c364-0695-4ec6-8b92-4c1db7c80f1b')/decisions",
    "@odata.count": 2,
    "value": [
        {
            "id": "4db68765-472d-4aa2-847a-433ea94bcfaf",
            "accessReviewId": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/bf59c5ba-5304-4c9b-9192-e5a4cb8444e7",
            "resourceLink": "https://graph.microsoft.com/v1.0/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
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
                "id": "eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
                "displayName": "Building security",
                "type": "group"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "bf59c5ba-5304-4c9b-9192-e5a4cb8444e7",
                "displayName": "Alex Wilber",
                "type": "user",
                "userPrincipalName": "AlexW@Contoso.com",
                "lastUserSignInDateTime": "2/11/2022 5:31:37 PM +00:00"
            }
        },
        {
            "id": "c7de8fba-4d6a-4fab-a659-62ff0c02643d",
            "accessReviewId": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
            "resourceLink": "https://graph.microsoft.com/v1.0/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
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
                "id": "eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
                "displayName": "Building security",
                "type": "group"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
                "displayName": "Adele Vance",
                "type": "user",
                "userPrincipalName": "AdeleV@Contoso.com",
                "lastUserSignInDateTime": "2/11/2022 4:58:13 PM +00:00"
            }
        }
    ]
}
```

从调用中， **决策** 属性具有其值 `NotReviewed` ，因为组成员尚未完成自我证明。 按照步骤 7 了解每个成员如何自我证明其访问评审需求。

## <a name="step-7-self-review-a-pending-access-decision"></a>步骤 7：自行审查挂起的访问决策

在步骤 3 中，你将访问评审配置为自审。 此配置要求 **生成安全** 组的两个成员自行证明其保持对组的访问权限的需要。

>[!NOTE]
>作为 **生成安全** 组的两个成员之一完成此步骤。

在此步骤中，你将列出挂起的访问评审，然后完成自证明过程。 可以使用 API 或使用 [“我的访问”门户](https://myaccess.microsoft.com/)，通过两种方式之一完成此步骤。 另一个审阅者不会完成此过程，而是允许将默认决策应用于其访问评审。

启动新的 **隐身**、 **匿名** 或 **InPrivate 浏览** 器会话，并作为 **生成安全** 组的两个成员之一登录。 这样做不会中断当前的管理员会话。 我们将以阿黛尔·万斯的身份登录。 或者，可以通过注销 Graph 资源管理器并作为两个组成员之一重新登录来中断当前管理员会话。

### <a name="method-1-use-the-access-reviews-api-to-self-review-pending-access"></a>方法 1：使用访问评审 API 对挂起的访问进行自我评审

#### <a name="list-your-access-reviews-decision-items"></a>列出访问评审决策项

在此调用中，请替换 `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` 为访问评审计划定义的 ID。

##### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/v1.0/identitygovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/decisions/filterByCurrentUser(on='reviewer')
```

##### <a name="response"></a>响应
从下面的响应中，你 (Adele Vance) 有一个挂起的访问评审， (**决定** `NotReviewed`) 自我证明。 **主体** 和 **资源** 属性指示决策适用的主体以及正在审查访问权限的资源。 在这种情况下，阿黛尔·万斯和 **建筑安全** 组分别。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(accessReviewInstanceDecisionItem)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
            "id": "c7de8fba-4d6a-4fab-a659-62ff0c02643d",
            "accessReviewId": "2d56c364-0695-4ec6-8b92-4c1db7c80f1b",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "principalLink": "https://graph.microsoft.com/v1.0/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
            "resourceLink": "https://graph.microsoft.com/v1.0/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
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
                "id": "eb75ccd2-59ef-48b7-8f76-cc3f33f899f4",
                "displayName": "Building security",
                "type": "group"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "3b8ceebc-49e6-4e0c-9e14-c906374a7ef6",
                "displayName": "Adele Vance",
                "type": "user",
                "userPrincipalName": "AdeleV@Contoso.com",
                "lastUserSignInDateTime": "2/15/2022 9:35:23 AM +00:00"
            }
        }
    ]
}
```

#### <a name="record-a-decision"></a>记录决策

若要完成访问评审，Adele Vance 将确认需要维护对 **Building 安全组的访问** 权限。

##### <a name="request"></a>请求

在此调用中，请替换 `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` 为访问评审计划定义的 ID 以及 `c7de8fba-4d6a-4fab-a659-62ff0c02643d` 上一步骤中返回的挂起决策项的 ID。

```http
PATCH https://graph.microsoft.com/v1.0/identitygovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/decisions/c7de8fba-4d6a-4fab-a659-62ff0c02643d

{
    "decision": "Approve",
    "justification": "As the assistant security manager, I still need access to the building security group."
}
```

##### <a name="response"></a>响应

```http
HTTP/1.1 204 No Content
```


#### <a name="verify-the-decisions"></a>验证决策

若要验证为访问评审记录的决策， [请列出访问评审决策项](#list-your-access-reviews-decision-items)。 虽然访问评审期尚未过期，也未应用决策，但 **applyResult** 将被标记为 `New` 允许更改决策。

现在可以注销并退出隐身浏览器会话。

### <a name="method-2-use-the-my-access-portal"></a>方法 2：使用“我的访问”门户

审阅者还可以访问 [“我的访问”门户](https://myaccess.microsoft.com/) 门户，以检查其挂起的访问评审实例。

+ 列出挂起的访问评审。 用户可以遵循以下两种方法之一来实现此目的：
  + 选项 1：从邮件收件箱中收到的电子邮件通知中选择 **“查看访问** ”按钮。 电子邮件通知类似于以下屏幕截图。 选择此按钮会将它们定向到挂起的访问评审。

  :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/emailnotification.png" alt-text="电子邮件通知以查看访问权限。" border="true":::

  + 选项 2：转到 [“我的访问”门户](https://myaccess.microsoft.com/) 。 选择 **“访问评审** ”菜单，然后选择“ **组和应用”** 选项卡。

+ 从访问评审列表中，选择要发布决策的访问评审。 选择 **“是** ”可发布仍需要访问 **“生成安全** 性”的决策。 输入原因，然后选择 **“提交**”。

  :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/selfattest.png" alt-text="自我证明需要维护对资源的访问权限。":::


现在可以注销并退出隐身浏览器会话。

## <a name="step-8-confirm-the-decisions-and-the-status-of-the-access-review"></a>步骤 8：确认访问评审的决定和状态

回到仍以全局管理员身份登录的主浏览器会话中，重复步骤 4 以查看 Adele Vance 的 **决策** 属性现在 `Approve`。 访问评审结束或过期时，将记录 Alex Wilber 的 `Deny` 默认决策。 然后会自动应用决策，因为 **autoApplyDecisionsEnabled** 已设置为 `true` 访问评审实例的期限将结束。 然后，Adele 将保持对 **Building 安全组的访问** 权限，Alex 将自动从该组中删除。

恭喜！ 你已创建访问评审，并根据维护访问权限的需要进行自我证明。 你只自我证明一次，并且将保持访问权限，直到通过另一个访问评审实例的决策或通过另一个 `Deny` 内部进程将其删除为止。

## <a name="step-9-clean-up-resources"></a>步骤 9：清理资源

删除为本教程创建的资源（ **生成安全** 组、访问评审计划定义和三个测试用户）。

### <a name="delete-the-security-group"></a>删除安全组

#### <a name="request"></a>请求

在此调用中，请替换`eb75ccd2-59ef-48b7-8f76-cc3f33f899f4`为 **生成安全** 性的 **ID**。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-delete_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/eb75ccd2-59ef-48b7-8f76-cc3f33f899f4
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="delete-the-access-review-definition"></a>删除访问评审定义

在此调用中，请替换 `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` 为访问评审定义的 ID。 由于访问评审计划定义是访问评审的蓝图，因此删除该定义将删除设置、实例和决策。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-delete_accessReviewScheduleDefinition"
}-->
```http
DELETE https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": false
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="delete-the-three-test-users"></a>删除三个测试用户
在此调用中，请替换 `3b8ceebc-49e6-4e0c-9e14-c906374a7ef6` 为其中一个测试用户的 ID。 使用其他两个用户的 ID 重复此步骤两次以删除它们。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-delete_user"
}-->
```http
DELETE https://graph.microsoft.com/beta/users/3b8ceebc-49e6-4e0c-9e14-c906374a7ef6
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

## <a name="conclusion"></a>结论

你已创建一个访问评审，在该评审中，主体已自我证明其需要维护对资源的访问权限（在本例中为 **生成安全** 组）。

本教程通过 Azure AD 访问评审 API 演示了其中一种方案。 访问评审 API 通过资源、主体和审阅者的组合来支持不同的方案，以满足访问证明需求。 有关详细信息，请参阅 [访问评审 API](/graph/api/resources/accessreviewsv2-overview)。

## <a name="see-also"></a>另请参阅

+ [什么是 Azure AD 访问评审？](/azure/active-directory/governance/access-reviews-overview)
+ [在 Azure AD 访问评审中自行查看对组或应用程序的访问权限](/azure/active-directory/governance/review-your-access)