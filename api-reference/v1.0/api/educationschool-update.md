---
title: 更新 educationSchool 属性
description: 更新 school 对象的属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2bd875c4824296c1b5ccfc6bd3969010a00b4f3b
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38303102"
---
# <a name="update-educationschool-properties"></a>更新 educationSchool 属性

更新 school 对象的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
| :------------------------------------- | :------------------------------------------ |
| 委派（工作或学校帐户）     | 不支持。                              |
| 委派（个人 Microsoft 帐户） | 不支持。                              |
| 应用程序                            | EduRoster.ReadWrite.All                     |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```

## <a name="request-headers"></a>请求标头

| 标头        | 值                     |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |
| Content-Type  | application/json          |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性            | 类型                                               | 说明                        |
| :------------------ | :------------------------------------------------- | :--------------------------------- |
| displayName         | 字符串                                             | 学校的显示名称         |
| 说明         | 字符串                                             | 学校描述          |
| principalEmail      | 字符串                                             | 主体的电子邮件地址     |
| principalName       | 字符串                                             | 主体名称              |
| externalPrincipalId | 字符串                                             | 同步系统中主体的 ID。 |
| highestGrade        | 字符串                                             | 教授的最高年级。              |
| lowestGrade         | 字符串                                             | 教授的最低年级。               |
| schoolNumber        | 字符串                                             | 学校编号。                     |
| externalId          | 字符串                                             | 同步系统中学校的 ID。    |
| phone               | String                                             | 学校电话号码。            |
| address             | [physicalAddress](../resources/physicaladdress.md) | 学校地址。             |
| createdBy           | [identitySet](../resources/identityset.md)         | 创建了学校的实体。     |

## <a name="response"></a>响应

如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationSchool](../resources/educationschool.md) 对象。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面展示了示例请求。

# <a name="httptabhttp"></a>[HTTP](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/schools/{school-id}
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```

# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "id": "10002",
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "phone": "+1 (253) 555-0102"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
