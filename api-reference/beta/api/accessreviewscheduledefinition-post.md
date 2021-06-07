---
title: 创建 accessReviewScheduleDefinition
description: 创建新的 accessReviewScheduleDefinition 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: ba1ce2b94cef8b37da03c655ccc2a687c2557cfd
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2021
ms.locfileid: "52780832"
---
# <a name="create-accessreviewscheduledefinition"></a>创建 accessReviewScheduleDefinition

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.All  |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序                            | AccessReview.ReadWrite.All |

登录用户还必须具有允许其创建访问评审的目录角色。  有关详细信息，请参阅访问评审的角色和 [权限要求](../resources/accessreviewsv2-root.md)。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /identityGovernance/accessReviews/definitions
```
## <a name="request-headers"></a>请求标头
| 名称         | 说明 |
|:-------------|:------------|
|Authorization|Bearer {token}。必需。|
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供 [accessReview](../resources/accessreview.md) 对象的 JSON 表示形式。

下表显示了创建 accessReview 时接受的属性。

| 属性 | 类型 | 说明 |
|:-------------|:------------|:------------|
| displayName | String | 访问评审系列的名称。 必填。|
| descriptionForAdmins | string | 提供给管理员评价的上下文。 必填。 |
  descriptionForReviewers | string | 提供给审阅者的审阅上下文。 必填。 |
| 范围 | [accessReviewScope](../resources/accessreviewscope.md) | 定义在组中查看的用户范围。 请参阅  [accessReviewScope，](../resources/accessreviewscheduledefinition.md) 并了解如何 [配置访问评审定义的范围](/graph/accessreviews-scope-concept)。 必填。| 
| instanceEnumerationScope | [accessReviewScope](../resources/accessreviewscope.md) | 对于所有组评审，这将确定将审核哪些组的范围。 请参阅 [accessReviewScope，](../resources/accessreviewscheduledefinition.md) 并了解如何 [配置访问评审定义的范围](/graph/accessreviews-scope-concept)。| 
| settings | [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)| 访问评审系列的设置。 定期在此处确定。 请参阅 [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md)。 |
| reviewers | [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合 | 定义审阅者是谁。 如果未指定任何内容，则评论是自 (审阅用户自己的访问权限或) 。 请参阅 [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md)。 |


## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-create-an-access-review-on-a-group"></a>示例 1：在组上创建访问评审

这是一个创建具有以下设置的访问评审的示例：
+ 评价将审阅组的所有成员，其组 **ID 为** `02f3bafb-448c-487c-88c2-5fd65ce49a41` 。
+ 用户 ID 为审阅 **者** `398164b1-5196-49dd-ada2-364b49f99b27` 的特定用户。
+ 它每周重复一次，并无限期地继续。

#### <a name="request"></a>请求
在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Test create",
  "descriptionForAdmins": "New scheduled access review",
  "descriptionForReviewers": "If you have any questions, contact jerry@contoso.com",
  "scope": {
    "query": "/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [
    {
      "query": "/users/398164b1-5196-49dd-ada2-364b49f99b27",
      "queryType": "MicrosoftGraph"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 1,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-08T12:02:30.667Z"
      }
    }
  }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "29f2d16e-9ca6-4052-bbfe-802c48944448",
  "displayName": "Test create",
  "createdDateTime": "0001-01-01T00:00:00Z",
  "lastModifiedDateTime": "0001-01-01T00:00:00Z",
  "status": "NotStarted",
  "descriptionForAdmins": "Test create",
  "descriptionForReviewers": "Test create",
  "instanceEnumerationScope": null,
  "createdBy": {
    "id": "957f1027-c0ee-460d-9269-b8444459e0fe",
    "displayName": "MOD Administrator",
    "userPrincipalName": "admin@contoso.com"
  },
  "scope": {
    "query": "/groups/b74444cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [
    {
      "query": "/users/7eae986b-d425-48b2-adf2-3c777f4444f3",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 1,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1,
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
        "startDate": "2020-09-08",
        "endDate": null
      }
    },
  "applyActions": []
  }
}
```

### <a name="example-2-create-an-access-review-on-all-teams-with-inactive-guest-users"></a>示例 2：在具有非活动来宾用户的所有团队上创建访问评审

这是一个创建具有以下设置的访问评审的示例：
+ 该评论将审核具有非活动来宾用户的所有团队。 非活动期为自访问评审开始日期起 30 天。
+ 组所有者为审阅者，并分配回退审阅者。
+ 它每季度的第三天重复发生，并无限期地继续。
+ **autoApplyDecisionsEnabled** 设置为 ，将 `true` **defaultDecision 设置为** `Deny` 。

#### <a name="request"></a>请求
在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition_inactiveguests_M365"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Review inactive guests on teams",
  "descriptionForAdmins": "Control guest user access to our teams.",
  "descriptionForReviewers": "Information security is everyone's responsibility. Review our access policy for more.",
  "instanceEnumerationScope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team')')",
    "queryType": "MicrosoftGraph"
  },
  "scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "inactiveDuration": "P30D"
    },
  "reviewers": [
    {
      "query": "./owners",
      "queryType": "MicrosoftGraph"
    }
  ],
  "fallbackReviewers": [
    {
      "query": "/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
      "queryType": "MicrosoftGraph"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "recommendationsEnabled": true,
    "instanceDurationInDays": 3,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "dayOfMonth": 5,
        "interval": 3
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-05-04T00:00:00.000Z"
      }
    },
    "defaultDecisionEnabled": true,
    "defaultDecision": "Deny",
    "autoApplyDecisionsEnabled": true
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-inactiveguests-m365-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-inactiveguests-m365-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-inactiveguests-m365-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-inactiveguests-m365-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
  "id": "b0966e21-a01e-43c9-8f8b-9ba30ed5710a",
  "displayName": "Review inactive guests on teams",
  "createdDateTime": "2021-05-04T18:27:02.6719849Z",
  "lastModifiedDateTime": "2021-05-04T18:27:24.0889623Z",
  "status": "InProgress",
  "descriptionForAdmins": "Control guest user access to our teams.",
  "descriptionForReviewers": "Information security is everyone's responsibility. Review our access policy for more.",
  "createdBy": {
    "id": "fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
    "displayName": "MOD Administrator",
    "userPrincipalName": "admin@contoso.com"
  },
  "scope": {
    "@odata.type": "#microsoft.graph.accessReviewInactiveUsersQueryScope",
    "query": "./members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
    "queryType": "MicrosoftGraph",
    "queryRoot": null,
    "inactiveDuration": "P30D"
  },
  "instanceEnumerationScope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups?$filter=(groupTypes/any(c:c+eq+'Unified') and resourceProvisioningOptions/Any(x:x eq 'Team'))&$count=true",
    "queryType": "MicrosoftGraph",
    "queryRoot": null
  },
  "reviewers": [
    {
      "query": "./owners",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "backupReviewers": [],
  "fallbackReviewers": [
    {
      "query": "/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": true,
    "defaultDecision": "Deny",
    "instanceDurationInDays": 3,
    "autoApplyDecisionsEnabled": true,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "interval": 3,
        "month": 0,
        "dayOfMonth": 5,
        "daysOfWeek": [],
        "firstDayOfWeek": "sunday",
        "index": "first"
      },
      "range": {
        "type": "noEnd",
        "numberOfOccurrences": 0,
        "recurrenceTimeZone": null,
        "startDate": "2021-05-05",
        "endDate": null
      }
    },
    "applyActions": []
  }
}
```

### <a name="example-3-create-an-access-review-of-all-users-to-an-application"></a>示例 3：创建对应用程序的所有用户的访问评审

这是一个创建具有以下设置的访问评审的示例：
+ 该评论将审核用户对应用程序的访问权限。
+ 人员经理是审阅者，回退审阅者是组的成员。
+ 它每半年重复一次，自 startDate 起 1 年后结束。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accessReviewScheduleDefinition_allusers_M365_AADRole"
}-->
```http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions
Content-type: application/json

{
  "displayName": "Review employee access to LinkedIn",
  "descriptionForAdmins": "Review employee access to LinkedIn",
  "scope": {
    "@odata.type": "#microsoft.graph.principalResourceMembershipsScope",
    "principalScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/users",
        "queryType": "MicrosoftGraph"
      }
    ],
    "resourceScopes": [
      {
        "@odata.type": "#microsoft.graph.accessReviewQueryScope",
        "query": "/servicePrincipals/bae11f90-7d5d-46ba-9f55-8112b59d92ae",
        "queryType": "MicrosoftGraph"
      }
    ]
  },
  "reviewers": [
    {
      "query": "./manager",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "backupReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph"
    }
  ],
  "fallbackReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph"
    }
  ],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": true,
    "defaultDecision": "Recommendation",
    "instanceDurationInDays": 180,
    "autoApplyDecisionsEnabled": true,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "interval": 6,
        "dayOfMonth": 0
      },
      "range": {
        "type": "numbered",
        "startDate": "2021-05-05",
        "endDate": "2022-05-05"
      }
    }
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accessreviewscheduledefinition-allusers-m365-aadrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accessreviewscheduledefinition-allusers-m365-aadrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accessreviewscheduledefinition-allusers-m365-aadrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-accessreviewscheduledefinition-allusers-m365-aadrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewScheduleDefinition"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions/$entity",
  "id": "1f79f34b-8667-40d9-875c-893b630b3dec",
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
        "query": "/servicePrincipals/bae11f90-7d5d-46ba-9f55-8112b59d92ae",
        "queryType": "MicrosoftGraph",
        "queryRoot": null
      }
    ]
  },
  "reviewers": [
    {
      "query": "./manager",
      "queryType": "MicrosoftGraph",
      "queryRoot": "decisions"
    }
  ],
  "backupReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "fallbackReviewers": [
    {
      "query": "/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers",
      "queryType": "MicrosoftGraph",
      "queryRoot": null
    }
  ],
  "settings": {
    "instanceDurationInDays": 180,
    "recurrence": {
      "pattern": {
        "type": "absoluteMonthly",
        "interval": 6,
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
        "startDate": "2021-05-05",
        "endDate": "2022-05-05"
      }
    }
  }
}
```


<!--
{
  "type": "#page.annotation",
  "description": "Create accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
