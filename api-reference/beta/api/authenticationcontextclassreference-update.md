---
title: 更新 authenticationContextClassReference
description: 更新 authenticationContextClassReference 对象的属性。
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: dcc0a20ac8b10fc1b7fad3fa3472832036f70024
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547327"
---
# <a name="update-authenticationcontextclassreference"></a>更新 authenticationContextClassReference

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [authenticationContextClassReference 对象](../resources/authenticationcontextclassreference.md) 的属性。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）                    |
|:--------------------------------------|:---------------------------------------------------------------|
|委派（工作或学校帐户）     | Policy.ReadWrite.ConditionalAccess |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | Policy.ReadWrite.ConditionalAccess |

> [!NOTE]
> 此 API 有 [一个与](/graph/known-issues#permissions) 权限相关的已知问题。

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /identity/conditionalAccess/authenticationContextClassReferences/{id}
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明      |
|:--------------|:-----------------|
| Authorization | Bearer {token}。必需。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关属性的值。 未添加到请求正文的现有属性要么保留旧值，要么根据其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

有关属性的列表，请参阅 [authenticationContextClassReference](../resources/authenticationContextClassReference.md)。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "update_authenticationcontextclassreference"
}-->

```http
PATCH https://graph.microsoft.com/beta/identity/conditionalAccess/authenticationContextClassReferences/c1
Content-type: application/json

{
   "value": 
    [
      {
         "displayName": "Contoso trusted locations",
        "description": "Access is only allowed from trusted locations",
        "isAvailable": true
      }
    ]
}
```



### <a name="response"></a>响应

下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": false
} -->

```http
HTTP/1.1 204 No Content
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update authenticationContextClassReference",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
