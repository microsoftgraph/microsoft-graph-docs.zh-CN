---
title: 将 Identityprovider.read.all 添加到 b2cUserFlow
description: 将 Identityprovider.read.all 添加到 b2cUserFlow。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d873cb83984e9da8e58e377df4ad7257b8f6531c
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319665"
---
# <a name="add-identityprovider-to-a-b2cuserflow"></a>将 Identityprovider.read.all 添加到 b2cUserFlow

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [b2cUserFlow](../resources/b2cuserflows.md) 对象中添加标识提供程序。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）|IdentityUserFlow|
|委派（个人 Microsoft 帐户）| 不支持。|
|应用程序| IdentityUserFlow|

工作或学校帐户需要属于下列角色之一：

* 全局管理员
* 外部标识用户流管理员

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /b2cUserFlows/{id}/identityProviders/$ref
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---------------|:----------|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 `id` 要添加的 [IDENTITYPROVIDER.READ.ALL](../resources/identityprovider.md) 的 JSON 表示形式。 有关可用于用户流的标识提供程序的详细信息，请参阅 [identityProviders](../resources/identityprovider.md) API reference。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。 如果失败，将返回 `4xx` 错误并显示具体详细信息。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "update_b2cuserflows_identityprovider"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/identityProviders/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/beta/identityProviders/{id}"
}
```

### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
