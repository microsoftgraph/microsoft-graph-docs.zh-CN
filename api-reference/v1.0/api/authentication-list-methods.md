---
title: List 方法
description: 检索身份验证方法对象的列表。
localization_priority: Normal
author: mmcla
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 937fabdba7863e209140019effe7c28458ab65c8
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054628"
---
# <a name="list-methods"></a>List 方法

命名空间：microsoft.graph

检索身份验证 [方法对象](../resources/authenticationmethod.md) 的列表。

> **注意：** 仅返回 v1.0 上支持的方法。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

### <a name="permissions-acting-on-self"></a>自行操作的权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:---------------------------------------|:-------------------------|
| 委派（工作或学校帐户）     | UserAuthenticationMethod.Read、UserAuthenticationMethod.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持。 |

### <a name="permissions-acting-on-other-users"></a>对其他用户操作的权限

|权限类型      | 权限（从最低特权到最高特权）              |
|:---------------------------------------|:-------------------------|:-----------------|
| 委派（工作或学校帐户）     | UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | UserAuthenticationMethod.Read.All、UserAuthenticationMethod.ReadWrite.All |

对于管理员正在操作其他用户的委派方案，管理员需要下列 [角色之一](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#available-roles)：
* 全局管理员
* 全局读取者
* 特权身份验证管理员
* 身份验证管理员 (只能看到屏蔽的电话号码) 

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET /me/authentication/methods
GET /users/{id | userPrincipalName}/authentication/methods
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法不支持自定义响应的可选查询参数。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [authenticationMethod](../resources/authenticationmethod.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。


```msgraph-interactive
GET https://graph.microsoft.com/v1.0/me/authentication/methods
```

### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authenticationMethod",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.fido2AuthenticationMethod",
      "id": "-2_GRUg2-HYz6_1YG4YRAQ2",
      "displayName": "Red key",
      "creationDateTime": "2020-08-10T06:44:09Z",
      "aaGuid": "2fc0579f-8113-47ea-b116-555a8db9202a",
      "model": "NFC key",
      "attestationCertificates": [
          "dbe793efdf1945e2df25d93653a1e8a3268a9075"
      ],
      "attestationLevel": "attested"
    },
    {
    "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
    "id": "b5e01f81-1f81-b5e0-811f-e0b5811fe0b5",
    "displayName": "Jordan's Surface Book",
    "createdDateTime": "2020-11-27T23:12:49Z",
    "keyStrength": "normal"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List methods",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
