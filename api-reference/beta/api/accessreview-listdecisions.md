---
title: 列表 accessReview 决策
description: 在 Azure AD 中访问审阅功能，检索 accessReview 对象的决策。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4f89fdbce1c87ce9ef8a6ba8c5b7f9b7be410617
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927007"
---
# <a name="list-accessreview-decisions"></a>列表 accessReview 决策

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，检索[accessReview](../resources/accessreview.md)对象的决策。

请注意，不会进行定期访问回顾`decisions`关系。  相反，呼叫者必须导航`instance`关系，以查找`accessReview`访问审阅的当前或过去实例的对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | `AccessReview.Read.All`, `AccessReview.ReadWrite.All`.  登录的用户还必须在目录角色中允许他们阅读访问审阅。 |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews('{reviewId}')/decisions
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者\{标记\}。 必需。 |

## <a name="request-body"></a>请求正文
应提供没有请求正文。

## <a name="response"></a>响应
如果成功，此方法返回`200, OK`响应代码和响应正文中的[accessReviewDecision](../resources/accessreviewdecision.md)对象的数组。

## <a name="example"></a>示例
##### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_accessReview_decisions"
}-->
```http
GET https://graph.microsoft.com/beta/accessReviews('2b83cc42-09db-46f6-8c6e-16fec466a82d')/decisions
```

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
|[获取 accessReview](accessreview-get.md) |  [accessReview](../resources/accessreview.md) |  检索访问审阅。 |
|[列出我 accessReview 决策](accessreview-listmydecisions.md) |        [accessReviewDecision](../resources/accessreviewdecision.md)集合|    审阅者，以获取 accessReview 我决策。|
|[发送 accessReview 提醒](accessreview-sendreminder.md) |       无。   |   向审阅者的 accessReview 发送提醒。 |
|[停止 accessReview](accessreview-stop.md) |        无。   |   停止 accessReview。 |
|[重置 accessReview 决策](accessreview-reset.md) |        无。   |   重置正在进行 accessReview 决策。|
|[应用 accessReview 决策](accessreview-apply.md) |        无。   |   应用已完成 accessReview 从的决策。|


<!-- {
  "type": "#page.annotation",
  "description": "Get accessReview decisions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
