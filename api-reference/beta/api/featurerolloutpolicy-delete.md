---
title: 删除 featureRolloutPolicy
description: 删除 featureRolloutPolicy 对象。
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d7197ffff516b1343b14c6042480fd003a94fac6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436097"
---
# <a name="delete-featurerolloutpolicy"></a>删除 featureRolloutPolicy

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

删除 [featureRolloutPolicy](../resources/featurerolloutpolicy.md) 对象。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | Policy.ReadWrite.FeatureRollout |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
DELETE /directory/featureRolloutPolicies/{id}
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {code} |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "delete_featurerolloutpolicy"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/directory/featureRolloutPolicies/df85e4d9-e8c4-4033-a41c-73419a95c29c
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
  "description": "Delete featureRolloutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


