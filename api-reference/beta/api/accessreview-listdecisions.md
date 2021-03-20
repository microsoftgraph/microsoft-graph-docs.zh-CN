---
title: 列出 accessReview 决策
description: 在 Azure AD 访问评审功能中，检索 accessReview 对象的决策。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 74ac3d2d9ec8857333beb94d8c5c96f1c4684c6b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943161"
---
# <a name="list-accessreview-decisions"></a>列出 accessReview 决策

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，检索 [accessReview 对象](../resources/accessreview.md) 的决策。

请注意，定期访问评审没有 `decisions` 关系。  相反，调用方必须导航 `instance` 关系以查找访问评审 `accessReview` 的当前或过去实例的对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.Read.All、AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | AccessReview.Read.All、AccessReview.ReadWrite.Membership |

 登录用户还必须具有允许其阅读访问评审的目录角色。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews/{reviewId}/decisions
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
不应提供请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `200, OK` [accessReviewDecision](../resources/accessreviewdecision.md) 对象数组。

## <a name="example"></a>示例
##### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/decisions
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreview-decisions-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreview-decisions-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreview-decisions-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreview-decisions-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewDecision",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
    {
            "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "accessReviewId": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
            "reviewResult": "Approve",
            "userPrincipalName": "alice@litware.com",
            "userId": "Alice Smith"
    }
    ]
}
```

## <a name="see-also"></a>另请参阅

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[获取 accessReview](accessreview-get.md) |  [accessReview](../resources/accessreview.md) |  检索访问评审。 |
|[列出我的 accessReview 决策](accessreview-listmydecisions.md) |        [accessReviewDecision](../resources/accessreviewdecision.md) 集合|    作为审阅者，获取我在 accessReview 上的决定。|
|[发送 accessReview 提醒](accessreview-sendreminder.md) |       无。   |   向 accessReview 的审阅者发送提醒。 |
|[Stop accessReview](accessreview-stop.md) |        无。   |   停止 accessReview。 |
|[重置 accessReview 决策](accessreview-reset.md) |        无。   |   重置进行中的 accessReview 中的决策。|
|[应用 accessReview 决策](accessreview-apply.md) |        无。   |   从已完成的 accessReview 应用决策。|


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


