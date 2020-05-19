---
title: servicePrincipal： removeKey
description: 从 servicePrincipal 中删除密钥凭据
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5ecd0f982bfa93c5ec3cf1125fb66f357b55948f
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289989"
---
# <a name="serviceprincipal-removekey"></a>servicePrincipal： removeKey

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

从[servicePrincipal](../resources/serviceprincipal.md)中删除密钥凭据。 ServicePrincipal 可以使用此方法和[addKey](serviceprincipal-addkey.md)自动滚动其过期密钥。

> [!NOTE]
> [Create servicePrincipal](../api/serviceprincipal-post-serviceprincipals.md) And [update servicePrincipal](../api/serviceprincipal-update.md)操作可继续用于添加和更新具有或不具有用户上下文的任何 servicePrincipal 的密钥凭据。

作为此方法的请求验证的一部分，在可以执行操作之前，将验证已拥有现有密钥的证明。

## <a name="permissions"></a>权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 无。  |
|委派（个人 Microsoft 帐户） | 无。    |
|应用程序 | 无。 |

> [!NOTE]
> ServicePrincipal 不需要任何特定权限即可滚动其自己的键。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /serviceprincipals/{id}/removeKey
```

## <a name="request-headers"></a>请求标头

| 名称           | 说明                |
|:---------------|:---------------------------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type   | application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供以下必需属性。

| 属性  | 类型 | 说明|
|:----------|:-----|:-----------|
| keyId     | GUID | 密码的唯一标识符。|
| 证明 | String | 自签名的 JWT 令牌，用作已有密钥的所有权证明。 必须使用 servicePrincipal 的现有有效证书之一的私钥对此 JWT 令牌进行签名。 令牌应包含以下声明：<ul><li>`aud`-需要访问群体 `00000002-0000-0000-c000-000000000000` 。</li><li>`iss`-颁发者需要是正在进行呼叫的 servicePrincipal 的__id__ 。</li><li>`nbf`-不早时间。</li><li>`exp`-过期时间应为 "nbf" + 10 分钟。</li></ul><br>下面是可用于生成此已占有令牌证明的代码[示例](/graph/application-rollkey-prooftoken)。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 No content` 响应代码。

## <a name="examples"></a>示例

以下示例演示如何调用此 API。

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "serviceprincipal_removekey"
}-->

```http
POST https://graph.microsoft.com/beta/serviceprincipals/{id}/removeKey
Content-Type: application/json

{
    "keyId": "f0b0b335-1d71-4883-8f98-567911bfdca6",
    "proof":"eyJ0eXAiOiJ..."
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

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "servicePrincipal: removeKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->