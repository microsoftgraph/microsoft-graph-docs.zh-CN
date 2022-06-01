---
title: '列出已弃用 (accessReviews) '
description: 检索 businessFlowTemplate 的 accessReview 对象。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 916229324c87bf4d7423dde0af86f6434e7cdef7
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65819124"
---
# <a name="list-accessreviews-deprecated"></a>列出已弃用 (accessReviews) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer](../../includes/accessreviews-disclaimer.md)]

检索特定 [businessFlowTemplate](../resources/businessflowtemplate.md) 的 [accessReview](../resources/accessreview.md) 对象。 对于使用该业务流模板创建的每次一次性和定期访问评审，将返回零个或多个 **accessReview** 对象的列表。  请注意，业务流模板 ID 区分大小写。

>[!NOTE]
> 如果与筛选器匹配的任何访问评审都是定期访问评审，则除了任何当前、过去和下一个即将推出的实例外，还将返回一个 **accessReview** 对象来表示每个定期序列作为一个整体。 例如，如果每月对组 A 的来宾成员进行定期访问评审、对 B 组的来宾成员进行季度定期访问评审，以及对组 C 的来宾成员进行一次性访问评审，则每个定期访问都刚刚开始，并且调用方使用组的来宾成员评审的业务流模板查询访问评审， 将返回三个表示三个序列的对象，以及当前访问评审实例的三个对象，以及下一个即将推出的实例的三个对象。 若要检索定期访问评审的实例或计划用于特定月份或季度的访问评审实例，调用方随后可以导航定期 **accessReview** 对象的 **实例** 关系。 实 **例** 关系链接到 **AccessReview** 对象，以获取定期访问评审的当前或过去实例。

如果许多访问评审与筛选器匹配，为了提高效率和避免超时，请在页面中检索结果集，方法是同时 `$top` 包括页面大小为 100 的查询参数和 `$skip=0` 请求中的查询参数。 即使未预料到请求将跨越多个页面，也可以包含这些参数。 当结果集跨多个页面时，Microsoft Graph在响应中返回包含`@odata.nextLink`下一页结果 URL 的属性的页面。 如果该属性存在，请继续使用每次响应中的 `@odata.nextLink` URL 来创建额外请求，直至返回所有结果，如[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)一文中所述。

此 API 返回的 **accessReview** 对象将不包括嵌套结构属性，例如 **设置** 或关系。  若要检索访问评审设置或关系，请使用 [get accessReview](accessreview-get.md) API。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.Read.All、AccessReview.ReadWrite.Membership、AccessReview.ReadWrite.All  |
|委派（个人 Microsoft 帐户） | 不支持。 |
|应用程序                            | AccessReview.Read.All、AccessReview.ReadWrite.Membership |

 已登录的用户还必须具有允许他们读取访问评审的目录角色。

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
请勿提供请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [accessReview](../resources/accessreview.md) 对象数组。

## <a name="examples"></a>示例
##### <a name="request"></a>请求
以下示例演示了检索业务流模板“6e4f3d20-c5c3-407f-9695-8460952bcc68”的所有一次性和定期访问评审的请求。

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


