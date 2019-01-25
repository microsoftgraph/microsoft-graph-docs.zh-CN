---
title: 获取 accessReview
description: '在 Azure AD 中访问审阅功能，检索 accessReview 对象。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 26551f27fdf328865509cd02011f3ee2344f5e82
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529143"
---
# <a name="get-accessreview"></a>获取 accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，检索[accessReview](../resources/accessreview.md)对象。  

若要检索访问审阅的审阅者，请使用[列表 accessReview 审阅者](accessreview-listreviewers.md)API。 若要检索访问审阅的决策，请使用[列表 accessReview 决策](accessreview-listdecisions.md)API 或[列出我 accessReview 决议](accessreview-listmydecisions.md)API。

如果这是定期访问回顾，然后使用`instances`关系，以检索过去，当前和将来实例访问审阅[accessReview](../resources/accessreview.md)集合。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | `AccessReview.Read.All`, `AccessReview.ReadWrite.All`.  登录的用户也必须在允许他们阅读访问审阅，或作为上访问审阅审阅者分配的目录角色。 |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者令牌 必需。 |

## <a name="request-body"></a>请求正文
应提供没有请求正文。

## <a name="response"></a>响应
如果成功，此方法返回`200, OK`响应代码和响应正文中的[accessReview](../resources/accessreview.md)对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')
```

##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
    "displayName": "review",
    "startDateTime": "2017-11-14T01:14:54.89Z",
    "endDateTime": "2017-12-14T01:14:54.89Z",
    "status": "InProgress",
    "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "reviewerType": "self",
    "description": "",
    "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"},
    "settings": {
        "mailNotificationsEnabled": true,
        "remindersEnabled": true,
        "justificationRequiredOnApproval": true,
        "autoReviewEnabled": false,
        "activityDurationInDays": 30,
        "autoApplyReviewResultsEnabled": false,
        "accessRecommendationsEnabled": false,
        "recurrenceSettings": {
            "recurrenceType": "onetime",
            "recurrenceEndType": "endBy",
            "durationInDays": 0,
            "recurrenceCount": 0
        },
        "autoReviewSettings": {
            "notReviewedResult": "Deny"
        }
    }
}
```

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建 accessReview](accessreview-create.md) |    [accessReview](../resources/accessreview.md) |  创建新 accessReview。 |
|[列表 programControls](programcontrol-list.md) | [programControl](../resources/programcontrol.md)集合 | 列出 programControls 租户中。 |
|[列表 accessReview 审阅者](accessreview-listreviewers.md) |     [userIdentity](../resources/useridentity.md)集合|    要获取 accessReview 审阅的者。 |
|[列表 accessReview 决策](accessreview-listdecisions.md) |     [accessReviewDecision](../resources/accessreviewdecision.md)集合|    获取 accessReview 的决策。|
|[列出我 accessReview 决策](accessreview-listmydecisions.md) |        [accessReviewDecision](../resources/accessreviewdecision.md)集合|    审阅者，以获取 accessReview 我决策。|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/accessreview-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
