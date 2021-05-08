---
title: 列出 administrativeUnit an educationSchool
description: 获取与 educationSchool 对象关联的 administrativeUnits 列表。
author: mmast
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 5cd736b14be199f729556c619015ab5fee1e857b
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232177"
---
# <a name="list-administrativeunit-an-educationschool"></a>列出 administrativeUnit an educationSchool

命名空间：microsoft.graph

获取与 [educationSchool](../resources/educationschool.md)对象关联的 **administrativeUnits** 列表。
## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | EduRoster.ReadBasic                         |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用程序                            | EduRoster.Read.All、EduRoster.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->

```http
GET /education/schools/{educationSchoolId}/administrativeUnit
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [administrativeUnit](../resources/administrativeunit.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "list_administrativeunit"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit
```

### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.administrativeUnit)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.administrativeUnit",
      "id": "03e281d6-81d6-03e2-d681-e203d681e203",
      "deletedDateTime": "String (timestamp)",
      "displayName": "String",
      "description": "String",
      "visibility": "String"
    }
  ]
}
```
