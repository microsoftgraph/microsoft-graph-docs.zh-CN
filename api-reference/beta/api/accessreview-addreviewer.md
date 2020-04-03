---
title: 添加 accessReview 审阅者
description: '在 "Azure AD access 评论" 功能中，更新现有的 accessReview 对象以将其他用户添加为审阅者。  仅允许对尚未完成的访问权限审核执行此操作，并且仅适用于显式指定审阅者的访问审核。 此操作不允许用于用户查看其自己的访问权限的访问审核，而不适用于将组所有者分配为审阅者的访问审核。 '
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ddda92a89f31035ec6900393018c77bd10c93ef1
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43123655"
---
# <a name="add-accessreview-reviewer"></a>添加 accessReview 审阅者

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 "Azure AD [access 评论](../resources/accessreviews-root.md)" 功能中，更新现有的[accessReview](../resources/accessreview.md)对象以将其他用户添加为审阅者。  仅允许对尚未完成的访问权限审核执行此操作，并且仅适用于显式指定审阅者的访问审核。 此操作不允许用于用户查看其自己的访问权限的访问审核，而不适用于将组所有者分配为审阅者的访问审核。 


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview、AccessReview 和所有 |
|委派（个人 Microsoft 帐户） | 不支持。 |
|Application                            | AccessReview.ReadWrite.Membership |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews/{reviewId}/reviewers
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供将成为审阅者的用户 ID 的 JSON 表示形式。

下表显示了在更新 accessReview 时可提供的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| `id`        | `String`   | 用户 ID。|


## <a name="response"></a>响应
如果成功，此方法将`201, Created`返回响应代码。

## <a name="example"></a>示例

以下是使用其他审阅者更新一次性（不定期）访问评审的示例。

##### <a name="request"></a>请求
在请求正文中，提供 user 对象的 id 的 JSON 表示形式。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "add_accessReview_reviewer"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews/2b83cc42-09db-46f6-8c6e-16fec466a82d/reviewers
Content-Type: application/json

{
    "id":"006111db-0810-4494-a6df-904d368bd81b"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-accessreview-reviewer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-accessreview-reviewer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-accessreview-reviewer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 201 Created
```

<!--
{
  "type": "#page.annotation",
  "description": "Add accessReview reviewer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
