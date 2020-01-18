---
title: 分配 tokenLifetimePolicy
description: 将 tokenLifetimePolicy 分配给应用程序或服务主体。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 5c68600b713d220468853bf56eaa6a136b647f8a
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234144"
---
# <a name="assign-tokenlifetimepolicy"></a>分配 tokenLifetimePolicy

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

将[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)分配给[应用程序](../resources/application.md)或[servicePrincipal](../resources/servicePrincipal.md)。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Policy. All 和 Application。所有读写。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | Policy. All 和 Application.readwrite.ownedby，all 和应用程序的 Read. all |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/tokenLifetimePolicies/$ref
POST /servicePrincipals/{id}/tokenLifetimePolicies/$ref
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 {token} |
| Content-Type | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供应分配给应用[](../resources/tokenlifetimepolicy.md)程序或服务主体的`@odata.id` tokenLifetimePolicy 对象的标识符（使用属性）。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_application"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/tokenLifetimePolicies
Content-Type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/policies/tokenLifetimePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
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
  "description": "Assign tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->