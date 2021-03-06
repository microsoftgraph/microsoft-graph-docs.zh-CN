---
title: 更新 accessReviewScheduleDefinition
description: 更新现有 accessReviewScheduleDefinition 对象以更改其一个或多个属性。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: be3b7603419d616ef9ea9e4da94fdb8942dc36f3
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030444"
---
# <a name="update-accessreviewscheduledefinition"></a>更新 accessReviewScheduleDefinition

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新现有 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象以更改其一个或多个属性。

>[!NOTE]
>对 accessReviewScheduleDefinition 进行的任何更新都仅适用于将来实例。 当前运行的实例无法更新。
>此外，此 API 不用于更新 accessReviewInstance 级别的属性（包括决策）。 有关[实例详细信息，请参阅 accessReviewInstance。](../resources/accessreviewinstance.md)

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序                            | AccessReview.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PUT /identityGovernance/accessReviews/definitions/{review-id}
```
## <a name="request-headers"></a>请求标头
| 名称         | 说明 |
|:-------------|:------------|
|Authorization|Bearer {token}。必需。|
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文
在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。

下表显示接受用于更新 accessReviewScheduleDefinition 的属性。

| 属性 | 类型 | 说明 |
|:-------------|:------------|:------------|
| displayName | String | 访问评审系列的名称。 |
| descriptionForAdmins | String | 提供给管理员评价的上下文。 |
| descriptionForReviewers | String | 提供给审阅者的审阅上下文。 |
| settings | [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md) | 访问评审系列的设置。 请参阅 [accessReviewScheduleSettings](../resources/accessreviewscheduledefinition.md)。 |
| reviewers | [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|  定义审阅者是谁。 如果未指定任何内容，则评论是自 (用户查看自己的访问权限) 。 只有在 **将** 单个用户分配为审阅者时，审阅者属性才可更新。 请参阅 [accessReviewReviewerScope](../resources/accessreviewscheduledefinition.md)。 |
|fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|用于定义回退审阅者列表的审阅者范围的集合，如果从指定的审阅者列表中找不到用户，将通知这些审阅者采取措施。 当组所有者指定为审阅者，但组所有者不存在时，或者将经理指定为审阅者但用户的经理不存在时，可能会发生这种情况。|
| backupReviewers (弃用) |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此属性已被 **fallbackReviewers 取代**。 但是，指定 **backupReviewers** 或 **fallbackReviewers** 会自动向另一个属性填充相同的值。 |

**PUT** 请求希望传入完整的对象，其中包括所有可写属性，而不只是要更新的属性。

## <a name="response"></a>响应
如果成功，此方法返回 响应 `204 No Content` 代码，无响应正文。

## <a name="examples"></a>示例

这是更新现有访问评审系列的 displayName 的示例。

### <a name="request"></a>请求
在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的新属性的 JSON 表示形式。



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewScheduleDefinition"
}-->
```http
PUT https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6

{
  "id": "60860cdd-fb4d-4054-91ba-f75e04444aa6",
  "displayName": "Test world UPDATED NAME!",
  "descriptionForAdmins": "Test world",
  "descriptionForReviewers": "Test world",
  "scope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "instanceEnumerationScope": {
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f",
    "queryType": "MicrosoftGraph"
  },
  "reviewers": [],
  "settings": {
    "mailNotificationsEnabled": true,
    "reminderNotificationsEnabled": true,
    "justificationRequiredOnApproval": true,
    "defaultDecisionEnabled": false,
    "defaultDecision": "None",
    "instanceDurationInDays": 3,
    "autoApplyDecisionsEnabled": false,
    "recommendationsEnabled": true,
    "recurrence": {
      "pattern": {
        "type": "weekly",
        "interval": 1
      },
      "range": {
        "type": "noEnd",
        "startDate": "2020-09-15"
      }
    }
  }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewScheduleDefinition",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
