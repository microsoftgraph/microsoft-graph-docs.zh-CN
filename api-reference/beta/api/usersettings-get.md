---
title: 获取设置
description: 阅读用户和组织设置对象。
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 309e27bd0cc197347ebd87aec6d1a968586ab167
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60935156"
---
# <a name="get-settings"></a>获取设置

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取用户和组织 [userSettings](../resources/usersettings.md) 对象若要了解如何更新 [userSettings](../resources/usersettings.md) 对象的属性，请参阅[更新用户设置](usersettings-update.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委托（工作或学校帐户） | User.Read.All、User.ReadWrite.All    |
|委托（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | User.Read.All,User.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

```http
GET /me/settings/
```

具有“用户ID”或“userPrincipalName”的请求只能由用户或具有 User.ReadWrite.All 权限的用户访问。若要了解详细信息，请参阅[权限](/graph/permissions-reference)。

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [userSettings](../resources/usersettings.md) 对象。

## <a name="example"></a>示例

##### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a>响应

这是一个示例响应。注意：为提高可读性，可能缩短了此处显示的响应对象。

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```


