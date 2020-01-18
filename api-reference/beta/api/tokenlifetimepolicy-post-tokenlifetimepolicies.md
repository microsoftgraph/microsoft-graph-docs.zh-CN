---
title: 创建 tokenLifetimePolicy
description: 创建新的 tokenLifetimePolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d40146e205dd250f99df3334b5e0c8d0323564c7
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234190"
---
# <a name="create-tokenlifetimepolicy"></a>创建 tokenLifetimePolicy

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建新的[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象。

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
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | 持有者 {token} |
| Content-type | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象的 JSON 表示形式。

## <a name="response"></a>响应

如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Create tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->