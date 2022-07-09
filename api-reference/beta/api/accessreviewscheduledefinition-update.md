---
title: 更新 accessReviewScheduleDefinition
description: 更新现有 accessReviewScheduleDefinition 对象以更改其一个或多个属性。
ms.localizationpriority: medium
author: zhusijia26
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a92ccb653267783c34206749c8f98e02e1f5becb
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696859"
---
# <a name="update-accessreviewscheduledefinition"></a>更新 accessReviewScheduleDefinition

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新现有 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象以更改其一个或多个属性。

>[!NOTE]
>对 accessReviewScheduleDefinition 所做的任何更新仅适用于将来的实例。 当前正在运行的实例无法更新。
>此外，此 API 不用于更新 accessReviewInstance 级别的属性（包括决策）。 有关实例的详细信息，请参阅 [accessReviewInstance](../resources/accessreviewinstance.md) 。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用                            | AccessReview.ReadWrite.All |

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

下表显示了接受的用于更新 accessReviewScheduleDefinition 的属性。

| 属性 | 类型 | 说明 |
|:-------------|:------------|:------------|
| descriptionForAdmins | 字符串 | 提供给管理员的评审的上下文。 |
| descriptionForReviewers | 字符串 | 提供给审阅者的审查的上下文。 |
| displayName | String | 访问评审系列的名称。 |
| fallbackReviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|用于定义回退审阅者列表的审阅者范围的集合，如果未从指定的审阅者列表中找到任何用户，则会通知他们采取行动。 如果组所有者被指定为审阅者，但组所有者不存在，或者经理被指定为审阅者，但用户的管理器不存在，则可能会发生这种情况。|
| 评论家 | [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|  定义审阅者是谁。 如果未指定任何内容，则评审是自审 (用户审阅自己的访问权限) 。 仅当将单个用户分配为审阅者时， **审阅者** 属性才可更新。 请参阅 [accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)。 |
|stageSettings|[accessReviewStageSettings](../resources/accessreviewstagesettings.md) 集合| 定义访问评审系列的每个实例将具有多少个阶段。 阶段将根据 **dependsOn** 属性按顺序创建。 每个阶段可以有不同的审阅者集、回退审阅者和设置。 只有审阅者和回退审阅者是可更新的。 请参阅 [accessReviewStageSettings](../resources/accessreviewstagesettings.md)。 可选。|
| settings | [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md) | 访问评审系列的设置。 请参阅 [accessReviewScheduleSettings](../resources/accessreviewschedulesettings.md)。 |
| backupReviewers (已弃用) |[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合| 此属性已替换为 **fallbackReviewers**。 但是，指定 **backupReviewers** 或 **fallbackReviewers** 会自动将相同的值填充到另一个属性。 |

**PUT** 请求要求传入完整的对象，其中包括所有可写属性，而不仅仅是要更新的属性。

## <a name="response"></a>响应
如果成功，此方法将返回响应代码，而不返回 `204 No Content` 响应正文。

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
Content-type: application/json

{
  "id": "60860cdd-fb4d-4054-91ba-f75e04444aa6",
  "displayName": "Test world UPDATED NAME!",
  "descriptionForAdmins": "Test world",
  "descriptionForReviewers": "Test world",
  "scope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
    "query": "/groups/b7a059cb-038a-4802-8fc9-b9d1ed0cf11f/transitiveMembers",
    "queryType": "MicrosoftGraph"
  },
  "instanceEnumerationScope": {
    "@odata.type": "#microsoft.graph.accessReviewQueryScope",
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
