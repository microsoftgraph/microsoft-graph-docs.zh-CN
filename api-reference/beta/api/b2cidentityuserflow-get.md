---
title: 获取 b2cIdentityUserFlow
description: 检索 b2cIdentityUserFlow 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4ef6d1b45e1f577a6538998eab74a569ff51125e
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48961205"
---
# <a name="get-b2cidentityuserflow"></a>获取 b2cIdentityUserFlow

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [b2cUserFlow](../resources/b2cidentityuserflow.md) 对象的属性和关系。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|IdentityUserFlow、IdentityUserFlow 和所有|
|委派（个人 Microsoft 帐户）| 不支持。|
|应用程序|IdentityUserFlow、IdentityUserFlow 和所有|

工作或学校帐户需要属于下列角色之一：

* 全局管理员
* 外部标识用户流管理员

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /identity/b2cUserFlows/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数

您可以使用 `$expand` 展开默认情况下不展开的特定用户流属性。

有关详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---------------|:----------|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [B2CIDENTITYUSERFLOW](../resources/b2cidentityuserflow.md) 的 JSON 表示形式。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_b2cUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-b2cuserflows-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-b2cuserflows-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-b2cuserflows-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-b2cuserflows-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2C_1_CustomerSignUp",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get b2cUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_b2cUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->


