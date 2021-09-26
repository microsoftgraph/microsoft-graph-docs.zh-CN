---
title: 列出 identityUserFlowAttributes
description: 检索 identityUserFlowAttribute 对象的列表。
ms.localizationpriority: medium
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: fd7d9809d417ca9824d7f29c1471f53197d496a8
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763483"
---
# <a name="list-identityuserflowattributes"></a>列出 identityUserFlowAttributes

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [identityUserFlowAttribute 对象](../resources/identityuserflowattribute.md) 的列表。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All|
|委派（个人 Microsoft 帐户）| 不支持。|
|应用程序|IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All|

工作或学校帐户需要属于以下角色之一：

* 全局管理员
* 外部标识用户Flow属性管理员

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---------------|:----------|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#userFlowAttributes",
    "value": [
      {
          "id": "City",
          "displayName": "City",
          "description": "Your city",
          "userFlowAttributeType": "builtIn",
          "dataType": "string"
      },
      {
          "id": "extension_d09380e2b4c6429a203fb816a04a7ad_Hobby",
          "displayName": "Hobby",
          "description": "Your hobby",
          "userFlowAttributeType": "custom",
          "dataType": "string",
      },
    ]
}
```
