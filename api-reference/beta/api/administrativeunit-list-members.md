---
title: 列出成员
description: 使用此 API 获取管理单元中的成员列表 (用户和组)。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b156079035b2f2332d81e018eba40bced41d9aee
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322791"
---
# <a name="list-members"></a>列出成员

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用此 API 获取管理单元中的成员列表 (用户和组)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | Directory.Read.All、Directory.ReadWrite.All |

> 注意: 若要在管理单元中列出隐藏成员身份的成员, 则需要使用 Read. hidden 权限是必需的。

## <a name="http-request"></a>HTTP 请求

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[user](../resources/user.md)和/或[group](../resources/group.md)对象的集合。  相反, 如果放`$ref`在请求的末尾, 则响应将包含成员的链接/url 的`@odata.id`集合。

## <a name="examples"></a>示例
##### <a name="list-member-objects"></a>列出成员对象
以下请求将列出管理单元的成员, 并返回用户和/或组的集合。

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.type":"#microsoft.graph.user",
      "id":"492c5308-59fd-4740-9c83-4b3db07a6d70"
      "accountEnabled":true,
      "businessPhones":[],
      "companyName":null,
      "displayName":"Demo User"
    },
    {
      "@odata.type":"#microsoft.graph.group",
      "id":"07eaa5c7-c9b6-45cf-8ff7-3147d5122caa",
      "description":"This group is the best ever",
      "displayName":"Awesome group"
    }
  ]
}
```

##### <a name="list-member-references"></a>列出成员引用
下面的请求将列出管理单元的成员引用, 并返回对成员的`@odata.id`引用集合。
```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
 
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/beta/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```
