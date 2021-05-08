---
title: 获取 educationSchool
description: 读取 educationSchool 对象的属性和关系。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 21732795ec15c16a92563eccebdeb7e8d33d3793
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231261"
---
# <a name="get-educationschool"></a>获取 educationSchool

命名空间：microsoft.graph

读取 [educationSchool 对象的属性和](../resources/educationschool.md) 关系。

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
GET /education/schools/{educationSchoolId}
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持与 Get User 相同的 OData [查询参数](../api/user-get.md#optional-query-parameters)。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称          | 说明               |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationSchool](../resources/educationschool.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_educationschool"
}
-->

```http
GET https://graph.microsoft.com/v1.0/education/schools/{educationSchoolId}
```

### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
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
}
```
