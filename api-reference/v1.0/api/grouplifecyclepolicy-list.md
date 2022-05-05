---
title: 列出 groupLifecyclePolicy
description: 列出所有 groupLifecyclePolicy。
author: psaffaie
ms.localizationpriority: medium
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 30ab8ceefd94400549c46dbb088a77bcc54f334f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209399"
---
# <a name="list-grouplifecyclepolicies"></a>列出 groupLifecyclePolicy

命名空间：microsoft.graph

列出所有 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）   |
| :------------------------------------- | :-------------------------------------------- |
| 委派（工作或学校帐户）     | Directory.Read.All 或 Directory.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。                                |
| Application                            | Directory.Read.All 或 Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /groupLifecyclePolicies
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) 对象集合。

## <a name="example"></a>示例

##### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_grouplifecyclepolicy_2"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/groupLifecyclePolicies
```

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-2-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/get-grouplifecyclepolicy-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-2-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/get-grouplifecyclepolicy-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-2-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/get-grouplifecyclepolicy-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicy-2-java-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/java/get-grouplifecyclepolicy-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-grouplifecyclepolicy-2-go-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/go/get-grouplifecyclepolicy-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-grouplifecyclepolicy-2-powershell-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/powershell/get-grouplifecyclepolicy-2-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应

注意：为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
      "groupLifetimeInDays": 100,
      "managedGroupTypes": "Selected",
      "alternateNotificationEmails": "admin@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List groupLifecyclePolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
