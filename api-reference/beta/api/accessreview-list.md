---
title: 列出 accessReviews
description: 检索 businessFlowTemplate 的 accessReview 对象。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a29d365a253f5917d3f5f58021dbe639d2a02713
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095131"
---
# <a name="list-accessreviews"></a>列出 accessReviews

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索特定[businessFlowTemplate](../resources/businessflowtemplate.md)的[accessReview](../resources/accessreview.md)对象。 对于使用该业务流程模板创建的每次一次性和定期访问评审，将返回零个或多个 **accessReview** 对象的列表。  请注意，业务流程模板的 ID 区分大小写。

>[!NOTE]
> 如果与筛选器匹配的任何访问评审是定期访问评审，则除了任何当前、过去和下一个即将发生的实例之外，还将返回一 **个 accessReview** 对象以表示整个定期系列。 例如，如果每月对组 A 的来宾成员进行定期访问评审，对组 B 的来宾成员进行季度定期访问评审，对组 C 的来宾成员进行一次性访问评审，则每个定期访问评审都刚刚开始，并且调用方使用查看组来宾成员的业务流程模板查询访问评审， 将返回表示三个系列的三个对象，以及当前访问评审实例的三个对象，以及下一个即将推出的实例可能返回的三个对象。 若要检索定期访问评审的实例，或为特定月份或季度安排的访问评审实例，调用方随后可以导航定期 **accessReview** 对象的实例关系。  实例 **关系** 链接到定期访问评审的当前或过去实例的 **accessReview** 对象。

如果许多访问评审与筛选器匹配，为了提高效率并避免超时，请检索页面中的 结果集，方法包括页面大小为 100 的查询参数和请求中的 query 参数。 `$top` `$skip=0` 即使您预计请求将跨越多个页面，也可以包含这些参数。 当一结果集跨多个页面时，Microsoft Graph 返回该页面，该页面在响应中包含指向下一页结果的 `@odata.nextLink` URL 中的属性。 如果该属性存在，请继续使用每次响应中的 `@odata.nextLink` URL 来创建额外请求，直至返回所有结果，如[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)一文中所述。

此 API 返回的 **accessReview** 对象不包括嵌套结构属性，如 **设置** 或 关系。  若要检索访问评审设置或关系，请使用 [get accessReview](accessreview-get.md) API。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.Read.All、AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | AccessReview.Read.All、AccessReview.ReadWrite.Membership |

 登录用户还必须具有允许其阅读访问评审的目录角色。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /accessReviews?$filter=businessFlowTemplateId eq {businessFlowTemplate-id}&$top={pagesize}&$skip=0
```
## <a name="request-headers"></a>请求标头
| 名称         | 类型        | 说明 |
|:-------------|:------------|:------------|
| Authorization | string | 持有者 \{token\}。必需。 |

## <a name="request-body"></a>请求正文
不提供请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReview](../resources/accessreview.md) 对象数组。

## <a name="examples"></a>示例
##### <a name="request"></a>请求
以下示例显示检索业务流程模板"6e4f3d20-c5c3-407f-9695-8460952bcc68"的所有一次性和定期访问评审的请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessReviews"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/accessReviews?$filter=businessFlowTemplateId+eq+'6e4f3d20-c5c3-407f-9695-8460952bcc68'&$top=100&$skip=0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviews-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviews-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviews-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviews-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-accessreviews-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-accessreviews-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



---


##### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReview",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value":[
       {
         "id": "2b83cc42-09db-46f6-8c6e-16fec466a82d",
         "displayName": "review",
         "startDateTime": "2017-11-14T01:14:54.89Z",
         "endDateTime": "2017-12-14T01:14:54.89Z",
         "status": "InProgress",
         "businessFlowTemplateId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
         "reviewerType": "self",
         "description": "",
         "reviewedEntity":{"id":"3b4f7e74-eb82-4120-9ff5-ba429c1ea6df","displayName":"Salesforce"}
       }
    ]
}
```

## <a name="see-also"></a>另请参阅

- [获取 accessReview](accessreview-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "Get accessReviews",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


