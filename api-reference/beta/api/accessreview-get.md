---
title: 获取 accessReview
description: '在 "Azure AD 访问评论" 功能中, 检索 accessReview 对象。  '
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 0bb757e3f92ced3d6f9615cb92a8e9b622bdec50
ms.sourcegitcommit: 4bdcb5cd3227ff009e10868f2936b3153372b87a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/25/2019
ms.locfileid: "33299575"
---
# <a name="get-accessreview"></a>获取 accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 "Azure AD[访问评论](../resources/accessreviews-root.md)" 功能中, 检索[accessReview](../resources/accessreview.md)对象。  

若要检索访问评审的审阅者, 请使用[列表 accessReview 审阅者](accessreview-listreviewers.md)API。 若要检索访问评审的决策, 请使用[list accessReview 决策](accessreview-listdecisions.md)api 或[list my accessReview 决策](accessreview-listmydecisions.md)api。

如果这是定期访问审核, 则使用`instances`关系检索访问评审的过去、当前和未来实例的[accessReview](../resources/accessreview.md)集合。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | AccessReview  |

若要调用此 API, 登录用户还必须位于允许他们读取访问审核的目录角色中, 或者可以将用户作为访问评审的审阅者进行分配。  有关更多详细信息, 请参阅[access 评审](../resources/accessreviews-root.md)的角色和权限要求。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
不应提供请求正文。

## <a name="response"></a>响应
如果成功, 此方法在响应`200, OK`正文中返回响应代码和[accessReview](../resources/accessreview.md)对象。

## <a name="example"></a>示例
##### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_accessReview"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d
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
|[创建 accessReview](accessreview-create.md) |    [accessReview](../resources/accessreview.md) |  创建新的 accessReview。 |
|[列出 programControls](programcontrol-list.md) | [programControl](../resources/programcontrol.md)集合 | 列出租户中的 programControls。 |
|[列出 accessReview 审阅者](accessreview-listreviewers.md) |     [userIdentity](../resources/useridentity.md)集合|    获取 accessReview 的审阅者。 |
|[列出 accessReview 决策](accessreview-listdecisions.md) |     [accessReviewDecision](../resources/accessreviewdecision.md)集合|    获取 accessReview 的决策。|
|[列出我的 accessReview 决策](accessreview-listmydecisions.md) |        [accessReviewDecision](../resources/accessreviewdecision.md)集合|    作为审阅者, 请 accessReview 的决策。|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
