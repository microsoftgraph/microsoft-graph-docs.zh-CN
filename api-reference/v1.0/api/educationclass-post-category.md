---
title: 创建 educationCategory
description: 创建新类别。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 3677ad2537eebd5b305ed69e147e42b6a0a84ad6f4f00a3d4f2ae8cd50ba66d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54130938"
---
# <a name="create-educationcategory"></a>创建 educationCategory

命名空间：microsoft.graph

在[educationClass 上创建新的 educationCategory。](../resources/educationcategory.md) [](../resources/educationclass.md)

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | 不支持。 | 

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories/$entity
```
## <a name="request-headers"></a>请求标头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |
| Content-Type  | application/json  |

## <a name="request-body"></a>请求正文
在请求正文中，提供 [educationCategory](../resources/educationcategory.md) 对象的 JSON 表示形式。


## <a name="response"></a>响应
如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [educationCategory](../resources/educationcategory.md) 对象。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。
<!-- {
  "blockType": "request",
  "sampleKeys": ["60eaa744-aa87-4276-b985-1633683119f8"],
  "name": "create_educationcategory_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/60eaa744-aa87-4276-b985-1633683119f8/assignmentCategories/$entity
Content-type: application/json
Content-length: 33

{ 
  "displayName": "Quizzes"
}
```
在请求正文中，提供 [educationCategory](../resources/educationcategory.md) 对象的 JSON 表示形式。

### <a name="response"></a>响应
下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 120

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('60eaa744-aa87-4276-b985-1633683119f8')/assignmentCategories/$entity",
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


