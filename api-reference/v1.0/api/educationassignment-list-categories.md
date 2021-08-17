---
title: 列出类别
description: 列出与此工作分配关联的所有类别。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c5ece16448dd047fb263149682352cdc8ea400b4
ms.sourcegitcommit: 1e9a53e7b8e67349288f5cfbabe8355de83817b0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2021
ms.locfileid: "58367161"
---
# <a name="list-categories"></a>列出类别

命名空间：microsoft.graph

列出与工作分配关联的所有类别。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） |  EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite  |
|委派（个人 Microsoft 帐户） |  不支持。  |
|应用程序 | EduAssignments.ReadBasic.All、EduAssignments.ReadWriteBasic.All、EduAssignments.Read.All、EduAssignments.ReadWrite.All | 

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/categories
```
## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求头
| 标头       | 值 |
|:---------------|:--------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationCategory](../resources/educationcategory.md) 对象集合。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["1fdf61ee-c129-4960-9b7c-8df159aa64b0"],
  "name": "get_assignment_categories"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/a17025d0-62a8-4450-9e6e-db31d8c8feb8/assignments/1fdf61ee-c129-4960-9b7c-8df159aa64b0/categories
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-assignment-categories-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-assignment-categories-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-assignment-categories-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-assignment-categories-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
下面展示了示例响应。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes('a17025d0-62a8-4450-9e6e-db31d8c8feb8')/assignments('1fdf61ee-c129-4960-9b7c-8df159aa64b0')/categories",
    "value": [
        {
            "displayName": "Quizzes",
            "id": "9b8f8f88-ddfc-4aad-9fe9-280513fffc74"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories added to an assignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
