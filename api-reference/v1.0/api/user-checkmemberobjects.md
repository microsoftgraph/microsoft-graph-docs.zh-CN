---
title: 用户： checkMemberObjects
description: 检查指定用户对象的组或目录角色列表中的成员资格。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8bec7df1327ef3d04ba0b3121e04d2e446fcf190
ms.sourcegitcommit: c25828c596b7e0939fa164a3d7754722943152c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2019
ms.locfileid: "38757305"
---
# <a name="user-checkmemberobjects"></a>用户： checkMemberObjects

检查指定用户对象的组或目录角色列表中的成员资格。 此方法是可传递的。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | User.readbasic.all，user. all，All。<br><br>此外：<br><br><ul><li>如果检查组中的成员身份： Group. All、Group. ReadWrite。 All</li><li>如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</li><li>如果检查目录角色中的成员身份： RoleManagement 和目录角色： RoleManagement</li></ul>Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All  |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | User.readbasic.all、所有用户读写全部。 All<br>并<ul><li>如果检查组中的成员身份： Group. All、Group. ReadWrite。 All</li><li>如果检查管理单元的成员身份： AdministrativeUnit、AdministrativeUnit</li><li>如果检查目录角色中的成员身份： RoleManagement 和目录角色： RoleManagement</li></ul>Directory.Read.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /me/checkMemberObjects
POST /users/{id}/checkMemberObjects
```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
|:--------------|:--------------|
| Authorization | Bearer {token}。必需。 |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数    | 类型        | 说明 |
|:-------------|:------------|:------------|
|ids|String collection|一个集合，包含要检查其成员身份的目录角色的组、目录角色或 roleTemplate Id 的对象 Id。 最大可指定20个对象。|

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和新的 String collection 对象。

## <a name="examples"></a>示例

下面是一个如何调用此 API 的示例。

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_checkmemberobjects"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/checkMemberObjects
Content-type: application/json

{
  "ids": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
}
```

### <a name="response"></a>响应

下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "String",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0", 
    "62e90394-69f5-4237-9190-012177145e10"
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "user: checkMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
