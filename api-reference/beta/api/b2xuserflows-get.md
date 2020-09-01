---
title: 获取 b2xUserFlows
description: 检索 b2xUserFlow 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 50089ec092dfe9802c97d253f872e47470d2f0f6
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319668"
---
# <a name="get-b2xuserflow"></a>获取 b2xUserFlow

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [b2xUserFlow](../resources/b2xuserflows.md) 对象的属性和关系。

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
GET /identity/b2xUserFlows/{id}
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

如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [USERFLOWATTRIBUTE](../resources/b2xuserflows.md) 的 JSON 表示形式。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "get_b2xUserFlows"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2xUserFlows/{id}
```

### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "B2X_1_PartnerSignUp",
    "userFlowType": "signUpOrSignIn",
    "userFlowTypeVersion": 1
}
```

<!-- {
  "type": "#page.annotation",
  "description": "Get b2xUserFlow",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: get_b2xUserFlows/userFlowTypeVersion:\r\n      Expected type Single but actual was Int64. Property: userFlowTypeVersion, actual value: '1'"
  ]
}-->
