---
title: 停止 accessReview
description: 在 "Azure AD access 评论" 功能中, 停止当前处于活动状态的 accessReview。  目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。  (若要防止定期访问审核启动以后的实例, 请更新它以更改计划的结束日期)。  在访问审核停止后, 审阅者无法再提供输入, 并且可以应用访问审核决定。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6c1616e811f079726614757732d11cd09ec5ed49
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408774"
---
# <a name="stop-accessreview"></a>停止 accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中, 停止当前处于活动状态的[accessReview](../resources/accessreview.md)。  目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。  (若要防止定期访问审核启动以后的实例, 请[更新它](accessreview-update.md)以更改计划的结束日期)。  在访问审核停止后, 审阅者无法再提供输入, 并且可以应用访问审核决定。
## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview、AccessReview 和所有 |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | AccessReview 的成员资格  |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/stop
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。


## <a name="response"></a>响应
如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例
##### <a name="request"></a>请求

# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/stop
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/stop-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/stop-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/stop-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
