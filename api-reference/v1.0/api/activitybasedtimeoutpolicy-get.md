---
title: 获取 activityBasedTimeoutPolicy
description: 获取 activityBasedTimeoutPolicy 对象的属性。
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 0830ef84ca3082d5e47deeca9575fd4055d8c358
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442619"
---
# <a name="get-activitybasedtimeoutpolicy"></a>获取 activityBasedTimeoutPolicy

命名空间：microsoft.graph



获取 [activityBasedTimeoutPolicy 对象](../resources/activitybasedtimeoutpolicy.md) 的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | Policy.Read.All、Policy.ReadWrite.ApplicationConfiguration |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /policies/activityBasedTimeoutPolicies/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `$select` OData 查询参数以帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回响应 `200 OK` 代码和请求 [的 activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitybasedtimeoutpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/policies/activityBasedTimeoutPolicies/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitybasedtimeoutpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitybasedtimeoutpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitybasedtimeoutpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-activitybasedtimeoutpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

