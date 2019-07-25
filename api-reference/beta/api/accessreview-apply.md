---
title: 应用 accessReview
description: '在 "Azure AD 访问评论" 功能中, 应用已完成 accessReview 的决策。  目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。  '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1a4c94406afbba762f3c461c06f9ba8252a3cbbc
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856238"
---
# <a name="apply-accessreview"></a>应用 accessReview

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 "Azure AD[访问评论](../resources/accessreviews-root.md)" 功能中, 应用已完成[accessReview](../resources/accessreview.md)的决策。  目标对象可以是一次性访问评审, 也可以是定期访问评审的实例。  


在访问审核完成后, 因为它已达到结束日期或管理员手动停止, 且未为审阅配置自动应用, 所以您可以调用 Apply 以应用所做的更改。 在应用之前, 不会在源资源上显示有关删除访问权限的决策, 因此实例的用户将保留其组成员身份。 通过调用 apply, 评审的结果通过更新组或应用程序来实现。 如果在审阅中拒绝了用户的访问权限, 则当管理员调用此 API 时, Azure AD 将删除其成员身份或应用程序分配。 

在访问评审完成且配置了自动应用后, 评审的状态将从 "已完成" 更改为 "中间状态", 最后将更改为 "已应用的状态"。 您应该会看到已拒绝的用户 (如果有) 在几分钟内从资源组成员身份或应用分配中删除。

已配置的自动应用审阅, 或选择 "应用" 不会对源于内部部署目录或动态组的组产生影响。 如果要更改源于内部部署的组, 请下载结果并将这些更改应用于该目录中的组的表示形式。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/applyDecisions()
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。


## <a name="response"></a>响应
如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="see-also"></a>另请参阅

- [如何完成访问评审](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-azure-ad-controls-complete-access-review)

## <a name="example"></a>示例
##### <a name="request"></a>请求

# <a name="httptabhttp"></a>[HTTP.SYS](#tab/http)
<!-- {
  "blockType": "request",
  "name": "apply_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2975E9B5-44CE-4E71-93D3-30F03B5AA992/applyDecisions
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/apply-accessreview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/apply-accessreview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目标-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/apply-accessreview-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/apply-accessreview-java-snippets.md)]
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
  "description": "Apply accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
