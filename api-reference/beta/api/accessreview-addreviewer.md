---
title: '添加 accessReview 审阅者 (已弃用) '
description: '在 Azure AD 访问评审功能中，更新现有 accessReview 对象，将另一个用户添加为审阅者。  此操作仅适用于尚未完成的访问评审，并且仅允许在显式指定审阅者的访问评审中执行此操作。 此操作不允许用户在访问评审中审阅其自己的访问权限，并且不适用于将组所有者分配为审阅者的访问评审。 '
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 1f59b588bb1ae59b9c21ee35beed218b23479195
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819385"
---
# <a name="add-accessreview-reviewer-deprecated"></a>添加 accessReview 审阅者 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

在 Azure AD [访问评审](../resources/accessreviews-root.md) 功能中，更新现有 [accessReview](../resources/accessreview.md) 对象，将另一个用户添加为审阅者。  此操作仅适用于尚未完成的访问评审，并且仅允许在显式指定审阅者的访问评审中执行此操作。 此操作不允许用户在访问评审中审阅其自己的访问权限，并且不适用于将组所有者分配为审阅者的访问评审。 


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | AccessReview.ReadWrite.Membership |

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
在请求正文中，提供将担任审阅者的用户 ID 的 JSON 表示形式。

下表显示了更新 accessReview 时可以提供的属性。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
| id        | String   | 用户 ID。|


## <a name="response"></a>响应
如果成功，此方法将返回 `201 Created` 响应代码。

## <a name="example"></a>示例

这是更新一次性 (不重复) 使用其他审阅者进行访问评审的示例。

##### <a name="request"></a>请求
在请求正文中，提供用户对象 ID 的 JSON 表示形式。


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

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-accessreview-reviewer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/add-accessreview-reviewer-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/add-accessreview-reviewer-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应
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


