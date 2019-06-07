---
title: 'educationSchool: delta'
description: 获取新创建或更新的学校, 而无需对整个学校集合执行完全读取。
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ef31d8cfa9f7b3680c4371e87eb86a46051f75bf
ms.sourcegitcommit: a3cdbd21dd81ca0158d63a1725fa0bd1dc270618
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764736"
---
# <a name="educationschool-delta"></a>educationSchool: delta

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取新创建或更新的学校, 而无需对整个学校集合执行完全读取。 有关详细信息, 请参阅[使用 delta 查询](/graph/delta-query-overview)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                              |
| :------------------------------------- | :----------------------------------------------------------------------- |
| 委派（工作或学校帐户）     | Eduroster.read.all、User.readbasic.all、Eduroster.read.all 或 Eduroster.read.all              |
| 委派（个人 Microsoft 帐户） | 不支持。                                                           |
| 应用程序                            | Eduroster.read.all、Eduroster.read.all、All 或 Eduroster.read.all 的所有 User.readbasic.all |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /education/schools/{id}/delta
POST /education/me/schools/{id}/delta
POST /education/users/{id}/schools/{id}/delta

```

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
| :------------ | :------------ |
| Authorization | Bearer {code} |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功, 此方法在响应`200 OK`正文中返回响应代码和[educationSchool](../resources/educationschool.md)集合对象。

## <a name="example"></a>示例

以下示例演示如何调用此 API。

##### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "request",
  "name": "educationschool_delta"
}-->

```http
POST https://graph.microsoft.com/v1.0/education/schools/{id}/delta
```

##### <a name="response"></a>响应

下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 313

{
  "value": [
    {
      "principalEmail": "principalEmail-value",
      "principalName": "principalName-value",
      "externalPrincipalId": "externalPrincipalId-value",
      "lowestGrade": "lowestGrade-value",
      "highestGrade": "highestGrade-value",
      "schoolNumber": "schoolNumber-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
