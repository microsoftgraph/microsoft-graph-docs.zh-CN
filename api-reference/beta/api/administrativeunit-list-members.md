---
title: 列出成员
description: 使用此 API 获取成员列表 (管理单元中) 组和设备的成员列表。
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6a3e591e164f92557c1661a3f3c3318508d054e7
ms.sourcegitcommit: b19b19bf192688f4c513492e8391e4d8dc104633
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2022
ms.locfileid: "62878629"
---
# <a name="list-members"></a>列出成员

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用此 API 获取成员列表 (管理单元中) 组和设备的成员列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All |

> 注意：若要列出管理单元中隐藏成员身份的成员，需要 Member.Read.Hidden 权限。

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>HTTP 请求

```http
GET /administrativeUnits/{id}/members
GET /administrativeUnits/{id}/members/$ref
```
## <a name="optional-query-parameters"></a>可选的查询参数
如果不 (`$ref` ，此方法) [OData](/graph/query-parameters) 查询参数来帮助自定义响应，包括 `$search``$count``$filter`、 和 。 例如，还可以启用 OData 转换，以便仅获取作为管理单元成员的用户。 

`$search` 仅在 **displayName 和** **description 属性上** 受支持。 只有将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count` 时，才支持某些查询。 有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

## <a name="request-headers"></a>请求标头
| 标头      |值|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |
| ConsistencyLevel  | 最终。 当使用 `$search` 或 `$filter` 的特定用法时，需要此标头和 `$count`。 有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [user](../resources/user.md)、 [group](../resources/group.md) 或 [device](../resources/device.md) 对象集合。 在 `$ref` 请求末尾添加将返回仅 `@odata.id` 成员 URL 的集合。

## <a name="examples"></a>示例
### <a name="example-1-list-member-objects"></a>示例 1：列出成员对象

#### <a name="request"></a>请求
以下请求将列出管理单元的成员，并返回用户和/或组的集合。

```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members
```

#### <a name="response"></a>响应

下面展示了示例响应。 
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
 
```http
HTTP/1.1 200 OK
Content-type: application/json

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

### <a name="example-2-list-member-references"></a>示例 2：列出成员引用

#### <a name="request"></a>请求

以下请求将列出管理单元的成员引用，并返回 `@odata.id` 对成员的引用集合。

```
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
```

#### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
 
```http
HTTP/1.1 200 OK
Content-type: application/json

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


