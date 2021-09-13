---
title: 更新 accessReviewScheduleDefinition
description: 更新 accessReviewScheduleDefinition 对象的属性。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 19d7613e7b2dfd59c5ed0c92f88d36488bd16943
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59023085"
---
# <a name="update-accessreviewscheduledefinition"></a>更新 accessReviewScheduleDefinition
命名空间：microsoft.graph

更新 [accessReviewScheduleDefinition 对象](../resources/accessreviewscheduledefinition.md) 的属性。

对 accessReviewScheduleDefinition 的任何更新仅适用于将来的实例。 当前运行的实例无法更新。 此外，此 API 不用于更新 accessReviewInstance 级别的属性（包括决策）。 有关[实例详细信息，请参阅 accessReviewInstance。](../resources/accessreviewinstance.md)

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|AccessReview.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的 JSON 表示形式。

下表显示接受用于更新 accessReviewScheduleDefinition 的属性。

| 属性 | 类型 | 说明 |
|:-------------|:------------|:------------|
| displayName | String | 访问评审系列的名称。 |
| descriptionForAdmins | String | 提供给管理员评价的上下文。 |
| descriptionForReviewers | String | 提供给审阅者的审阅上下文。 |
| settings | [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md) | 访问评审系列的设置。 请参阅 [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)。 |
| reviewers | [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|  定义审阅者是谁。 如果未指定任何内容，则评论是自 (用户查看自己的访问权限) 。 只有在 **将** 单个用户分配为审阅者时，审阅者属性才可更新。 请参阅 [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)。 |
|fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|用于定义回退审阅者列表的审阅者范围的集合，如果从指定的审阅者列表中找不到用户，将通知这些审阅者采取措施。 当组所有者指定为审阅者但组所有者不存在时，或者将经理指定为审阅者但用户的经理不存在时，可能会发生这种情况。|

**PUT** 请求希望传入完整对象，其中包括所有可写属性，而不只是要更新的属性。

## <a name="response"></a>响应
如果成功，此方法返回 响应 `204 No Content` 代码，无响应正文。

## <a name="examples"></a>示例
这是更新现有访问评审系列的 displayName 的示例。

### <a name="request"></a>请求

在请求正文中，提供 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象的新属性的 JSON 表示形式。



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewscheduledefinition"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-f75e04444aa6
Content-type: application/json

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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewscheduledefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewscheduledefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewscheduledefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewscheduledefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
