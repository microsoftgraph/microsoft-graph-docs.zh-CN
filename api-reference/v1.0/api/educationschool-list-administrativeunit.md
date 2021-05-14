---
title: 列出 administrativeUnit an educationSchool
description: 获取与 educationSchool 对象关联的 administrativeUnits 列表。
author: mmast
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a8ca5a51c6fb71c3cab0d6f0a7be239eb2101999
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474848"
---
# <a name="list-administrativeunit-an-educationschool"></a>列出 administrativeUnit an educationSchool

命名空间：microsoft.graph

获取与 [educationSchool](../resources/educationschool.md)对象关联的 **administrativeUnits** 列表。
## <a name="permissions"></a>Permissions

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


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_administrativeunit"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/{educationClassId}/members/{educationUserId}/schools/{educationSchoolId}/administrativeUnit
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-administrativeunit-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-administrativeunit-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-administrativeunit-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-administrativeunit-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
