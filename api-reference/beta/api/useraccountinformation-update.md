---
title: 更新 userAccountInformation
description: 更新 userAccountInformation 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 78d890a00916c72b8c48e5b41a1c84e1e2e2ffb8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938139"
---
# <a name="update-useraccountinformation"></a>更新 useraccountinformation

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新用户的[配置文件](../resources/profile.md)中的[userAccountInformation](../resources/useraccountinformation.md)对象的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 所有用户读写。          |
| 委派（个人 Microsoft 帐户） | 所有用户读写。          |
| 应用程序                            | User.ReadWrite.All                          |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /me/profile/account/{id}
```

## <a name="request-headers"></a>请求标头

| 名称           |说明                 |
|:---------------|:---------------------------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type   | application/json. 必需 |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性            | 类型                                    | 描述                                                                                    |
|:--------------------|:----------------------------------------|:-----------------------------------------------------------------------------------------------|
|ageGroup             |String                                   |显示用户的年龄组。 允许的`null`值`minor`、 `notAdult`和`adult`。 只读。 |
|countryCode          |字符串                                   |包含与用户帐户关联的双字符 countryCode。                       |
|preferredLanguageTag |[localeInfo](../resources/localeinfo.md) |包含用户与帐户相关的首选语言。                     |
|userPrincipalName    |字符串                                   |与帐户关联的用户的用户主体名称（UPN）。                          |

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[userAccountInformation](../resources/useraccountinformation.md)对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。
<!-- {
  "blockType": "request",
  "name": "update_useraccountinformation"
}-->

```http
PATCH https://graph.microsoft.com/beta/me/profile/account/{id}
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
  "description": "Update useraccountinformation",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
