---
title: 获取 userAccountInformation
description: 检索 useraccountinformation 对象的属性和关系。
localization_priority: Normal
author: kevinbellinger
ms.prod: Profile
doc_type: apiPageType
ms.openlocfilehash: a13208654b343fdff29b2495c58ebc54a168b52e
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937453"
---
# <a name="get-useraccountinformation"></a>获取 userAccountInformation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索[userAccountInformation](../resources/useraccountinformation.md)对象的属性和关系。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 不支持。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| Application                            | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /user/profile/account
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持一些 OData 查询参数来帮助自定义响应。 有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[userAccountInformation](../resources/useraccountinformation.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "get_useraccountinformation"
}-->

```http
GET https://graph.microsoft.com/Beta/user/profile/account
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.userAccountInformation"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "ageGroup": "ageGroup-value",
  "countryCode": "countryCode-value",
  "preferredLanguageTag": {
    "locale": "locale-value",
    "displayName": "displayName-value"
  },
  "userPrincipalName": "userPrincipalName-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get userAccountInformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
