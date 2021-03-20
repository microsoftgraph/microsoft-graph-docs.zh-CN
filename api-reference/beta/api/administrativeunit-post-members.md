---
title: 添加成员
description: 使用此 API 将用户或 (组的成员) 管理单元。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 9f3aca05107b73232b11e42ed70a9e737c65a45b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942938"
---
# <a name="add-a-member"></a>添加成员

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用此 API 将用户或 (组的成员) 管理单元。

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AdministrativeUnit.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | AdministrativeUnit.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
在请求正文中，提供 `id` 要[添加的用户、](../resources/user.md)[组](../resources/group.md)或[directoryObject](../resources/directoryobject.md)的 。

## <a name="response"></a>响应

如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面是一个请求示例。

<!-- {
  "blockType": "request",
  "name": "post_administrativeUnits_members"
} -->
```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
在请求正文中， `id` 提供 [要添加](../resources/user.md) 的用户或 [组](../resources/group.md) 对象的 。

### <a name="response"></a>响应
下面是一个响应示例。
 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```


