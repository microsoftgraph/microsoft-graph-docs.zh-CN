---
title: 获取设置
description: 读取用户和组织设置对象。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 128feebf624350baaea9fee41c411bd46c2b42c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32536559"
---
# <a name="get-settings"></a>获取设置

读取用户和组织[设置](../resources/user-settings.md)对象。
若要了解如何更新[settings](../resources/user-settings.md)对象的属性, 请参阅[更新用户设置](user-update-settings.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | User.Read.All、User.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | user. all、user. ReadWrite |

## <a name="http-request"></a>HTTP 请求

```http
GET /me/settings/
```

具有 "user id" 或 "userPrincipalName" 的请求只能由用户或具有用户的 ReadWrite 权限的用户访问。 若要了解详细信息, 请参阅[权限](/graph/permissions-reference)。

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[用户设置](../resources/user-settings.md)对象。

## <a name="example"></a>示例

##### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a>响应

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

