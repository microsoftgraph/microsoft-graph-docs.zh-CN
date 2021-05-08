---
title: 获取 educationClass
description: 从系统检索类
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 52f24e1f3c02b955874a78cdba447b697485f4a3
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232009"
---
# <a name="get-educationclass"></a>获取 educationClass

命名空间：microsoft.graph

从系统检索课程。 课程是带特殊属性的通用组，向系统表明该组是课程。 Group members represent the students;组管理员表示班级中的教师。 如果使用的是委派令牌，用户只会看到他们作为成员的课程。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  EduRoster.ReadBasic  |
|委派（个人 Microsoft 帐户） |  不支持  |
|应用程序 | EduRoster.Read.All、EduRoster.ReadWrite.All | 

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数
可以使用 `$select` 获取特定组属性，包括非默认返回的属性。

有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。
## <a name="request-headers"></a>请求头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。
## <a name="response"></a>响应
如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象。
## <a name="example"></a>示例
##### <a name="request"></a>请求
下面是一个请求示例。

如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}
-->

```http
GET /education/classes/{educationClassId}
```

### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationClass",
    "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
    "displayName": "String",
    "mailNickname": "String",
    "description": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "classCode": "String",
    "externalName": "String",
    "externalId": "String",
    "externalSource": "String",
    "externalSourceDetail": "String",
    "grade": "String",
    "term": {
      "@odata.type": "microsoft.graph.educationTerm"
    }
  }
}
```
