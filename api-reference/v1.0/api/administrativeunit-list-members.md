---
title: 列出成员
description: 使用此 API 获取管理单元中 (用户、组或设备) 的成员列表。
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4de66a36c8399a233b5dabdd65041415c2abfe42
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884295"
---
# <a name="list-members"></a>列出成员

命名空间：microsoft.graph

使用此 API 获取管理单元中 (用户、组或设备) 的成员列表。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All |

> 注意：若要列出管理单元中隐藏成员身份的成员，需要 Member.Read.Hidden 权限。

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a>HTTP 请求

```http
GET /directory/administrativeUnits/{id}/members
GET /directory/administrativeUnits/{id}/members/$ref
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法 (在没有) 的情况下`$ref`使用[时支持 OData 查询参数](/graph/query-parameters)，以帮助自定义响应，包括`$search``$count``$filter`和 。 OData 强制转换也已启用，例如，可以强制转换以仅获取属于管理单元成员的用户。 

`$search` 仅在 **displayName** 和 **description** 属性上受支持。 只有将 **ConsistencyLevel** 标头设置为 `eventual` 和 `$count` 时，才支持某些查询。 有关详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。

## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |
| ConsistencyLevel  | 最终。 当使用 `$search` 或 `$filter` 的特定用法时，需要此标头和 `$count`。 有关使用 **ConsistencyLevel** 和 `$count` 的详细信息，请参阅 [Azure AD 目录对象的高级查询功能](/graph/aad-advanced-queries)。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [用户](../resources/user.md)、 [组](../resources/group.md)或 [设备](../resources/device.md) 对象的集合。 在请求结束时添加 `$ref` 会返回仅 `@odata.id` 包含成员 URL 的集合。

## <a name="examples"></a>示例

### <a name="example-1-list-member-objects"></a>示例 1：列出成员对象

#### <a name="request"></a>请求
以下请求将列出管理单元的成员，并返回用户、组和设备的集合。

<!-- {
  "blockType": "request",
  "name": "list_administrativeunit_members"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/c5729e7c-988e-417b-b287-14f5bd4711d8/members
```

#### <a name="response"></a>响应
下面是一个响应示例。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.administrativeUnit)"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects",
    "value": [
        {
            "@odata.type": "#microsoft.graph.device",
            "id": "7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac",
            "accountEnabled": true,
            "deviceId": "6fa60d52-01e7-4b18-8055-4759461fc16b",
            "displayName": "Test Windows device",
            "operatingSystem": "Windows"
        },
        {
            "@odata.type": "#microsoft.graph.device",
            "id": "c530e1f6-7b4c-4313-840e-cf1a99ec3b38",
            "accountEnabled": false,
            "deviceId": "4c299165-6e8f-4b45-a5ba-c5d250a707ff",
            "displayName": "Test Linux device",
            "operatingSystem": "linux"
        }
    ]
}
```

### <a name="example-2-list-member-references"></a>示例 2：列出成员引用

#### <a name="request"></a>请求
以下请求将列出管理单元的成员引用，并返回对成员的 `@odata.id` 引用集合。

<!-- {
  "blockType": "request",
  "name": "list_administrativeunit_member_refs"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/{id}/members/$ref
```

#### <a name="response"></a>响应
下面是一个响应示例。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.administrativeUnit)"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value":[
    {
      "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/492c5308-59fd-4740-9c83-4b3db07a6d70"
    },
    {
      "@odata.id": "https://graph.microsoft.com/v1.0/directoryObjects/07eaa5c7-c9b6-45cf-8ff7-3147d5122caa"
    }
  ]
}
```
