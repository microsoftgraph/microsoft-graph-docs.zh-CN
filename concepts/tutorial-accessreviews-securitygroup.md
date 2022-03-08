---
title: 教程：使用访问评审 API 查看对安全组的访问权限
description: Azure AD安全组可用于控制对资源的访问。 使用访问评审 API 证明安全组的所有成员都需要其成员身份，并按扩展名访问分配给安全组的资源。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: governance
ms.openlocfilehash: ccb305df3cc5dbdf21d97ce1b87791a6729d5df8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337395"
---
# <a name="tutorial-use-the-access-reviews-api-to-review-access-to-your-security-groups"></a>教程：使用访问评审 API 查看对安全组的访问权限

Microsoft Graph 中的访问评审 API 使组织能够审核和证明标识 (也称为) 分配给组织中资源的访问权限。 通过安全组管理主体对其他资源的访问权限的最高效Azure AD之一。 例如，数百个用户可以分配给安全组，而为安全组分配文件夹访问权限。 通过使用访问评审 API，组织可以定期向有权访问此类组的主体以及组织中其他资源的主体提供证明。

假设您使用Azure AD组分配标识 (*也称为*) 访问组织中资源的主体。 需要定期证明安全组的所有成员都需要其成员身份，并按扩展名证明他们访问分配给安全组的资源。

本教程指导你使用访问评审 API 查看对租户中安全Azure AD的访问权限。 可以使用浏览器Graph Postman 尝试和测试访问评审 API 调用，然后再将它们自动化到脚本或应用中。 此测试环境有助于正确定义和验证查询，而无需重复地重新编译应用程序，从而节省时间。

## <a name="prerequisites"></a>先决条件

若要完成本教程，需要以下资源和权限：

+ 启用Azure AD EMS E5 Azure AD Premium P2工作租户。
+ 以全局[Graph](https://developer.microsoft.com/graph/graph-explorer)或标识管理管理员角色中的用户身份登录Azure AD资源管理器。
  + [可选]打开新的 **隐身、****匿名** 或 **InPrivate 浏览器** 窗口。 你将在本教程的稍后部分登录。
+ 以下委派权限：、`AccessReview.ReadWrite.All``Group.ReadWrite.All`。

若要同意在资源管理器中Graph权限：
1. 选择用户帐户详细信息右边的设置齿轮图标，然后选择" **选择权限"**。

    :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/settings.png" alt-text="选择&quot;microsoft Graph权限&quot;。" border="true":::

2. 滚动浏览这些权限的权限列表：
   + AccessReview (3) ，展开并选择 **AccessReview.ReadWrite.All**。
   + 将 (2) ，展开，然后选择 **Group.ReadWrite.All**。
  
    选择 **"** 同意"，然后在弹出窗口中，选择"代表你的组织同意"，然后选择"接受"以接受权限同意。

   :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/consentpermissions.png" alt-text="同意 Microsoft Graph权限。" border="true":::
   
>[!NOTE]
>为了可读性，本教程中显示的响应对象可能会缩短。
   
## <a name="step-1-create-test-users-in-your-tenant"></a>步骤 1：在租户内创建测试用户

通过运行以下请求三次，创建三个新的测试用户，每次更改 **displayName**、 **mailNickname** 和 **userPrincipalName** 属性的值。 记录三个新测试用户的 ID。

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

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
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

创建一个名为 **"构建** 安全性"的安全组，该组是本教程中访问评审的目标。 为此组分配一个组所有者和两个成员。

### <a name="request"></a>请求

在上一步中，创建了三个测试用户。 其中一个用户将是组所有者，而其他两个用户将是组的成员。

在此调用中，替换：
+ `d3bcdff4-4f80-4418-a65e-7bf3778c5dca` 使用组所有者的 ID。
+ `3b8ceebc-49e6-4e0c-9e14-c906374a7ef6` 以及 `bf59c5ba-5304-4c9b-9192-e5a4cb8444e7` 两个组的成员的 ID。

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

在响应中，记录新组的 ID，以在本教程的稍后部分使用它。

## <a name="step-3-create-an-access-review-for-the-security-group"></a>步骤 3：为安全组创建访问评审

### <a name="request"></a>请求

在此调用中，替换以下值：
+ `eb75ccd2-59ef-48b7-8f76-cc3f33f899f4` 具有"生成安全 **"组的** ID。 范围指定将审阅应用于 Building **安全组的** 所有成员。 有关配置范围的更多选项，请参阅另 [请参阅部分](#see-also) 。
+ **startDate** 的值，带今天的日期，值 **endDate**，其日期为开始日期 5 天。

访问评审具有以下设置：

+ 当你没有为 **reviewers** 属性指定值时，这是一种自审阅。 因此，每个组成员将自行证明其维护对组的访问权限需求。
+ 审查的范围是 (安全) 的 **直接或间接成员** 。
+ 审阅者必须提供他们为什么需要维护对组的访问权限的理由。
+ 默认决策是 `Deny` 当实例过期之前审阅者不响应访问评审请求时。 该 `Deny` 决定会从组中删除这些组的成员。
+ 这是一次一次访问评审，在五天后结束。 因此，授予访问权限后，用户无需在访问评审期间再次自行证明。
+ 在审查范围内定义的主体将收到电子邮件通知和提醒，提示他们自行证明其维护访问权限需求。

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

上述访问评审的状态标记为 **NotStarted**。 您可以在 GET (GET `https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b`) 检索访问评审，以监视状态，当其标记为 **InProgress** 时，即创建了访问评审的实例，可以发布决策。 您还可以检索访问评审以查看访问评审的完整设置。

## <a name="step-4-list-instances-of-the-access-review"></a>步骤 4：列出访问评审的实例

将 **访问** 评审的状态 `InProgress`标记为 后，运行以下查询以列出访问评审定义的所有实例。 由于在步骤 3 中创建了一次访问评审，因此请求仅返回一个 ID 与计划定义 ID 类似的实例。

### <a name="request"></a>请求

在此调用中，将 替换为 `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` 步骤 3 中返回的访问评审定义的 ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_accessReviewInstance"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances
```

### <a name="response"></a>响应

在此响应中， **实例** 的状态是 `InProgress` ， **因为 startDateTime** 已过去， **endDateTime** 在将来。 如果 **startDateTime** 在将来，则状态将为 `NotStarted`。 另一方面，如果 **endDateTime** 过去，状态将为 `Completed`。

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

## <a name="step-5-who-was-contacted-for-the-review"></a>步骤 5：Who评价的联系人？

您可以确认已联系 **Building 安全** 组的所有成员，以发布针对此访问评审实例的审阅决策。

### <a name="request"></a>请求

在此调用中，将 替换为 `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` 访问评审计划定义的 ID。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_contactedReviewers"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/contactedReviewers
```

### <a name="response"></a>响应

以下响应显示，"生成"安全组的 **两个成员收到** 有关其待审阅的通知。

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

对访问评审实例做出的决策感兴趣。

### <a name="request"></a>请求

在此调用中，将 替换为 `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` 访问评审计划定义的 ID 和实例。

<!-- {
  "blockType": "request",
  "name": "tutorial-accessreviews-Securitygroup-list_accessReviewInstanceDecisionItem"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/decisions
```

### <a name="response"></a>响应

以下响应显示了对审阅实例做出的决策。 由于 **构建安全性** 有两个成员，因此需要两个决策项。

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

在调用中 **，decision** 属性的值 `NotReviewed` 为 ，因为组的成员尚未完成自证明。 按照步骤 7 了解每个成员如何自行证明其访问评审需求。

## <a name="step-7-self-review-a-pending-access-decision"></a>步骤 7：自我审阅挂起的访问决策

在步骤 3 中，您将访问评审配置为自审阅。 此配置要求构建安全组的两个成员自行证明他们维护对组的访问权限。

>[!NOTE]
>作为"生成安全"组的两个成员之一 **完成** 此步骤。

在此步骤中，将列出待处理的访问评审，然后完成自证明过程。 可以通过以下两种方法之一完成此步骤：使用 API 或 [My Access 门户](https://myaccess.microsoft.com/)。 另一个审阅者不会完成此过程，相反，你将允许默认决策应用于其访问评审。

启动新的 **隐身****、匿名** 或 **InPrivate** 浏览浏览器会话，并作为构建安全组的两个成员 **之** 一登录。 这样，您就不会中断当前管理员会话。 我们将以 Adele Vance 登录。 或者，也可以中断当前管理员会话，Graph资源管理器中注销并作为两个组的成员之一重新登录。

### <a name="method-1-use-the-access-reviews-api-to-self-review-pending-access"></a>方法 1：使用访问评审 API 自行审阅待定访问权限

#### <a name="list-your-access-reviews-decision-items"></a>列出访问评审决策项

在此调用中，将 替换为 `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` 访问评审计划定义的 ID。

##### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/v1.0/identitygovernance/accessReviews/definitions/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/instances/2d56c364-0695-4ec6-8b92-4c1db7c80f1b/decisions/filterByCurrentUser(on='reviewer')
```

##### <a name="response"></a>响应
从下面的响应中， (Adele Vance) 有 `NotReviewed` 一个挂起的访问 (决定) 自行证明。 **主体****和资源** 属性指示决定适用于的主体以及正在审查其访问权限的资源。 在这种情况下，分别为 Adele Vance **和 Building 安全** 组。

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

若要完成访问评审，Adele Vance 将确认需要维护对"生成安全" **组** 的访问权限。

##### <a name="request"></a>请求

在此调用中，将 替换为 `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` 访问评审 `c7de8fba-4d6a-4fab-a659-62ff0c02643d` 计划定义的 ID 和上一步中返回的挂起决策项目的 ID。

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

若要验证为访问评审记录的决策，请 [列出访问评审决策项](#list-your-access-reviews-decision-items)。 虽然访问评审期尚未过期，也未应用决策， **但 applyResult** `New` 将被标记为 ，你可以更改决策。

现在可以注销并退出无法识别的浏览器会话。

### <a name="method-2-use-the-my-access-portal"></a>方法 2：使用"我的访问"门户

审阅者还可以访问 ["我的访问"门户](https://myaccess.microsoft.com/) 门户，以检查其挂起的访问评审实例。

+ 列出挂起的访问评审。 用户可以按照以下两种方法之一到达那里：
  + 选项 1： **从他们收到的邮件** 收件箱中的电子邮件通知中选择"查看访问"按钮。 电子邮件通知与以下屏幕截图类似。 选择此按钮会指导他们进行挂起的访问评审。

  :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/emailnotification.png" alt-text="查看访问权限的电子邮件通知。" border="true":::

  + 选项 2：转到 ["我的访问"门户](https://myaccess.microsoft.com/) 门户。 选择" **访问评审"** 菜单，然后选择" **组和应用"** 选项卡。

+ 从访问评审列表中，选择要发布其决策的访问评审。 选择 **"** 是"可发布你仍然需要访问"构建 **安全性"的决定**。 输入原因，**然后选择提交。**

  :::image type="content" source="../images/../concepts/images/tutorial-accessreviews-api/selfattest.png" alt-text="自我证明需要维护对资源的访问权限。":::


现在可以注销并退出无法识别的浏览器会话。

## <a name="step-8-confirm-the-decisions-and-the-status-of-the-access-review"></a>步骤 8：确认访问评审的决策和状态

返回到你仍以全局管理员身份登录的主浏览器会话中，重复步骤 4 以查看 Adele Vance 的决策属性现在为 。 `Approve` 当访问评审结束或过期时， `Deny` 将为 Alex Wilber 记录的默认决定。 然后，将自动应用决策，因为 **autoApplyDecisionsEnabled** `true` 已设置为 ，并且访问评审实例的时间段将结束。 然后，Adele 将维护对 **Building 安全** 组的访问权限，并且 Alex 将自动从该组中删除。

恭喜！ 你已创建访问评审并自行证明你维护访问需求。 你仅自证明一 `Deny` 次，并且将保持访问权限，直到通过其他访问评审实例的决定或其他内部进程将其删除。

## <a name="step-9-clean-up-resources"></a>步骤 9：清理资源

删除为本教程创建的资源-生成安全组、访问评审计划定义和三个测试用户。

### <a name="delete-the-security-group"></a>删除安全组

#### <a name="request"></a>请求

在此调用中，将 替换为`eb75ccd2-59ef-48b7-8f76-cc3f33f899f4`**"构建安全性****"的 ID**。

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

在此调用中，将 替换为 `2d56c364-0695-4ec6-8b92-4c1db7c80f1b` 访问评审定义的 ID。 由于访问评审计划定义是访问评审的蓝图，因此删除该定义将删除设置、实例和决策。

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
在此调用中，将 `3b8ceebc-49e6-4e0c-9e14-c906374a7ef6` 替换为测试用户之一的 ID。 对另外两个用户的 ID 重复此步骤两次以删除它们。

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

## <a name="conclusion"></a>结束语

你已创建访问评审，其中主体已自行证明需要维护对资源（本例中为"生成安全"组 **）的访问权限。**

本教程通过访问评审 API 演示了Azure AD之一。 访问评审 API 通过组合资源、主体和审阅者支持不同的方案，以满足你的访问证明需求。 有关详细信息，请参阅访问 [评审 API](/graph/api/resources/accessreviewsv2-overview?view=graph-rest-beta&preserve-view=true)。

## <a name="see-also"></a>另请参阅

+ [访问评审 API](/graph/api/resources/accessreviewsv2-overview?view=graph-rest-beta&preserve-view=true)
+ [访问Azure AD是什么？](/azure/active-directory/governance/access-reviews-overview)
+ [在访问评审中审阅自己对Azure AD的访问权限](/azure/active-directory/governance/review-your-access)