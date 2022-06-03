---
title: 获取成员
description: 使用此 API 在管理单元中获取特定成员 (用户、组或设备) 。
author: DougKirschner
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 5919b75724f10d16dbdca5669e511d9a24b67503
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2022
ms.locfileid: "65884223"
---
# <a name="get-a-member"></a>获取成员

命名空间：microsoft.graph

使用此 API 在管理单元中获取特定成员 (用户、组或设备) 。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All    |
|委派（个人 Microsoft 帐户） | 不支持。    |
|应用程序 | AdministrativeUnit.Read.All、Directory.Read.All、AdministrativeUnit.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

```http
GET /directory/administrativeUnits/{id}/members/{id}
```
## <a name="request-headers"></a>请求标头
| 名称      |说明|
|:----------|:----------|
| Authorization  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [用户](../resources/user.md)、 [组](../resources/group.md)或 [设备](../resources/device.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。

<!-- {
  "blockType": "request",
  "name": "get_administrativeunit_members"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/directory/administrativeUnits/c5729e7c-988e-417b-b287-14f5bd4711d8/members/7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac
```

### <a name="response"></a>响应
下面是一个响应示例。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.administrativeUnit"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#directoryObjects/$entity",
    "@odata.type": "#microsoft.graph.device",
    "id": "7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac",
    "accountEnabled": true,
    "createdDateTime": "2022-04-20T08:53:50Z",
    "deviceId": "6fa60d52-01e7-4b18-8055-4759461fc16b",
    "displayName": "Test device",
    "operatingSystem": "Windows"
}
```
