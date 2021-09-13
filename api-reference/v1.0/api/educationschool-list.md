---
title: 列出 educationSchools
description: 获取 educationSchool 对象及其属性的列表。
author: mlafleur
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 7e609820f4a6ca48acdc6522c6f141a0160dd4bf
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59022714"
---
# <a name="list-educationschools"></a>列出 educationSchools

命名空间：microsoft.graph

获取 [educationSchool 对象](../resources/educationschool.md) 及其属性的列表。

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
GET /education/schools
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持与 List Users 相同的 OData [查询参数](../api/user-list.md#optional-query-parameters)。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象的集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_educationschool"
}
-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/schools
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.educationSchool)"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.educationSchool",
      "id": "1c23c12e-c12e-1c23-2ec1-231c2ec1231c",
      "displayName": "String",
      "description": "String",
      "externalSource": "String",
      "externalSourceDetail": "String",
      "principalEmail": "String",
      "principalName": "String",
      "externalPrincipalId": "String",
      "lowestGrade": "String",
      "highestGrade": "String",
      "schoolNumber": "String",
      "externalId": "String",
      "phone": "String",
      "fax": "String",
      "createdBy": {
        "@odata.type": "microsoft.graph.identitySet"
      },
      "address": {
        "@odata.type": "microsoft.graph.physicalAddress"
      }
    }
  ]
}
```
