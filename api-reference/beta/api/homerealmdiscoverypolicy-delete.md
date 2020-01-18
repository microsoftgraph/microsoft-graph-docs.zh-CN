---
title: 删除 homeRealmDiscoveryPolicy
description: 删除 homeRealmDiscoveryPolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fc54623f6b30226adc493511c1dc8413b5e96421
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234171"
---
# <a name="delete-homerealmdiscoverypolicy"></a>删除 homeRealmDiscoveryPolicy

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | ApplicationConfiguration |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | ApplicationConfiguration |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /policies/homeRealmDiscoveryPolicies/{id}
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "delete_homerealmdiscoverypolicy"
}-->

```http
DELETE https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/{id}
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
  "description": "Delete homeRealmDiscoveryPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->