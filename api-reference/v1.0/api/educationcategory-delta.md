---
title: educationCategory： delta
description: 获取新创建或更新的 educationCategory 对象的列表，而无需对集合执行完整读取。
author: cristobal-buenrostro
ms.localizationpriority: medium
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6d14f74d8123c2be2754b62e4976b73d45080b07
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66445936"
---
# <a name="educationcategory-delta"></a>educationCategory： delta
命名空间：microsoft.graph

获取新创建或更新的 [educationCategory 对象的](../resources/educationcategory.md) 列表，而无需对集合执行完整读取。

> 此方法不会返回已删除的类别。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）                                                            |
| :------------------------------------- | :----------------------------------------------------------------------------------------------------- |
| 委派（工作或学校帐户）     | EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite |
| 委派（个人 Microsoft 帐户） | 不支持。                                                                                         |
| 应用程序                            | EduAssignments.ReadBasic.All、EduAssignments.ReadWriteBasic.All、EduAssignments.Read.All、EduAssignments.ReadWrite.All |

## <a name="optional-query-parameters"></a>可选的查询参数
此方法仅支持 `$top` OData 查询参数。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /education/classes/{educationClassId}/assignmentCategories/delta
GET /education/classes/{educationClassId}/assignments/{educationAssignmentId}/categories/delta
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回 `200 OK` 响应代码和 [educationCategory](../resources/educationcategory.md) 集合。

## <a name="examples"></a>示例

### <a name="example-1-get-assignment-categories"></a>示例 1：获取分配类别

#### <a name="request"></a>请求

下面展示了示例请求。

`$top`使用该参数指定要返回的类别数。 该参数是可选的。 如果有一长串类别，请使用它;否则，你将获取类中的所有类别。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classcategories_delta"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta?$top=3
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classcategories-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classcategories-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classcategories-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classcategories-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-classcategories-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-classcategories-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。 

>**注意：** 从响应中 `@odata.nextLink` 获取另一个调用并获取下一组类别。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationCategory)",
    "@odata.nextLink": "https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta?$skiptoken=U43TyYWKlRvJ6wWxZOfJvkp22nMqShRw9f-GxBtG2FDy9b1hMDaAJGdLb7n2fh1IVSFtBcXz0jxjIEihcR91dS3R7i8Z2IMtxIn9rKbK9Jvurj6jCH-lDbSNatdesrK0PJ5zpZ_-i8HyqkdtLhWD9tewXVArIqQWJA7gJz8z4paG2q0MU9rixrQOTe7WIXikPiBTUPilHuUW-o1k7cvqke3K7llJbU3G7z_O7WGoVGE.l8-2OcBi9ZWAhwhPnXvJ-kyyk8GNb6-H4o6qofP5YBY",
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationCategory",
            "displayName": "Fall 21",
            "id": "f0fd3e18-87a7-4060-b348-bd2d7a178a9d"
        },
        {
            "@odata.type": "#microsoft.graph.educationCategory",
            "displayName": "reading",
            "id": "10aa7bb1-7f5b-4c12-b1d4-0bf1429a12de"
        },
        {
            "@odata.type": "#microsoft.graph.educationCategory",
            "displayName": "expand",
            "id": "02f60051-806d-4729-a251-4156f7d8e8a5"
        }
    ]
}
```

### <a name="example-2-get-next-set-of-categories"></a>示例 2：获取下一组类别

#### <a name="request"></a>请求

下面展示了示例请求。

`@odata.nextLink`使用此请求的上一次调用中的值。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classcategories_delta"
}-->

```msgraph-interactive
GET /education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta?$skiptoken=U43TyYWKlRvJ6wWxZOfJvkp22nMqShRw9f-GxBtG2FDy9b1hMDaAJGdLb7n2fh1IVSFtBcXz0jxjIEihcR91dS3R7i8Z2IMtxIn9rKbK9Jvurj6jCH-lDbSNatdesrK0PJ5zpZ_-i8HyqkdtLhWD9tewXVArIqQWJA7gJz8z4paG2q0MU9rixrQOTe7WIXikPiBTUPilHuUW-o1k7cvqke3K7llJbU3G7z_O7WGoVGE.l8-2OcBi9ZWAhwhPnXvJ-kyyk8GNb6-H4o6qofP5YBY
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classcategories-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classcategories-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classcategories-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classcategories-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-classcategories-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-classcategories-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 必须继续使用后置调用 `@odata.nextLink` 的值，直到在响应中获取属性 `@odata.deltaLink` 。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationCategory)",
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta?$deltatoken=7ORzTfzlUEGDy6BRE3OC-3ePBbvLHCRe4aJ_hjaBKJxUHmn_ODgoM4xreLS7YRaxc-iACeqCQsT5Tb0u9vn6QXYflO6j0sRgRQlhcfR7DApZYl6uZqiXcR7H0G14btPqR761sKWNc0jgiczrHGF6dGfSQwsLzPT46og-84ArhOU.Jnxvkr08FE-QBvEYstYel3JZUrgwgTauo-GmpbdWeSA",
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationCategory",
            "displayName": "apps",
            "id": "62cee656-f3e7-45c9-958f-5dc3ff47dd97"
        },
        {
            "@odata.type": "#microsoft.graph.educationCategory",
            "displayName": "homework",
            "id": "440c56ea-6c2a-4566-a8ab-56fcda3bc1e3"
        }
    ]
}
```

### <a name="example-3-get-the-created-and-modified-categories-using-delta-token"></a>示例 3：使用增量令牌获取已创建和修改的类别

#### <a name="request"></a>请求

下面展示了示例请求。

`@odata.deltaLink`使用此请求的上一次调用中的值。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_classcategories_delta"
}-->

```msgraph-interactive
GET /education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta?$deltatoken=7ORzTfzlUEGDy6BRE3OC-3ePBbvLHCRe4aJ_hjaBKJxUHmn_ODgoM4xreLS7YRaxc-iACeqCQsT5Tb0u9vn6QXYflO6j0sRgRQlhcfR7DApZYl6uZqiXcR7H0G14btPqR761sKWNc0jgiczrHGF6dGfSQwsLzPT46og-84ArhOU.Jnxvkr08FE-QBvEYstYel3JZUrgwgTauo-GmpbdWeSA
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-classcategories-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-classcategories-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-classcategories-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-classcategories-delta-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-classcategories-delta-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-classcategories-delta-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 自初始 Delta 调用以来，必须继续使用该 `@odata.deltaLink` 类别获取新创建的或修改的类别。

>有时，增量响应会非常大，在这种情况下，将返回一个 `@odata.nextLink` 继续提取更改，直到再次命中 `@odata.deltaLink` 。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 344

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(educationCategory)",
    "@odata.deltaLink": "https://graph.microsoft.com/v1.0/education/classes/72a7baec-c3e9-4213-a850-f62de0adad5f/assignmentcategories/delta?$deltatoken=7ORzTfzlUEGDy6BRE3OC-3ePBbvLHCRe4aJ_hjaBKJxUHmn_ODgoM4xreLS7YRaxc-iACeqCQsT5Tb0u9vn6QXYflO6j0sRgRQlhcfR7DApVu5vuUKP3uuUhFpYW8Ku3RtYbkmxRlHbDAkK-NyvPczuDOJqONtesUhKgaoXQGmM.4Rw7IYlmUFBcaDmEbJoGDLMbchYNgoLiPNyp4e7z2po",
    "value": [
        {
            "@odata.type": "#microsoft.graph.educationCategory",
            "displayName": "arts",
            "id": "d9fa9b82-04d5-4411-ae4d-848e6fd75575"
        }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2021-11-18 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List categories: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
