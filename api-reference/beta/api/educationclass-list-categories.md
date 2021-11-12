---
title: 列出 assignmentCategories
description: 检索类别对象的列表。
author: mmast-msft
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 11a0087a3c120f8cc98d542bf90e4ed53a5a0ccc
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60936010"
---
# <a name="list-assignmentcategories"></a>列出 assignmentCategories

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [educationCategory 对象](../resources/educationcategory.md) 的列表。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| 委派（工作或学校帐户）     | EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。                                                                                         |
| 应用程序                            | EduAssignments.ReadBasic.All、EduAssignments.ReadWriteBasic.All、EduAssignments.Read.All、EduAssignments.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignmentCategories
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。

## <a name="request-headers"></a>请求头

| 标头        | 值                     |
| :------------ | :------------------------ |
| Authorization | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [educationCategory](../resources/educationcategory.md) 对象集合。

## <a name="example"></a>示例

##### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["4797d052-ebf5-4018-a088-e11adc6b2cbb"],
  "name": "get_class_categories"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/education/classes/4797d052-ebf5-4018-a088-e11adc6b2cbb/assignmentCategories
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-class-categories-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-class-categories-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-class-categories-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-class-categories-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>响应

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

{
    "@odata.context": "https://graph.microsoft.com/v1.0/education/classes('4797d052-ebf5-4018-a088-e11adc6b2cbb')/assignmentCategories",
    "value": [
      {
          "displayName": "Quizzes",
          "id": "f997a279-6bcf-429e-b1d0-d2320c4b84ab"
      },
      {
          "displayName": "Homework",
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
  "description": "List categories",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
