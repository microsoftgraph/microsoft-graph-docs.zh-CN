---
title: 列出 contactedReviewers
description: 获取访问评审实例的审阅者。
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 66ab5232af06485d2ae1cef688e7ed1e82ec4dff
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697531"
---
# <a name="list-contactedreviewers"></a>列出 contactedReviewers
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [访问评审实例的审阅](../resources/accessreviewinstance.md)者，无论他们是否收到通知。 审阅者由 [accessReviewReviewer](../resources/accessreviewreviewer.md) 对象表示。 返回零个或多个对象的列表，包括其所有嵌套属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|AccessReview.Read.All、AccessReview.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用|AccessReview.Read.All、AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/contactedReviewers
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select`OData `$skip``$filter``$orderBy`查询参数，`$top`以帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

此 API 的默认页面大小为 100 **个 accessReviewReviewer** 对象。 若要提高效率并避免因大型结果集而超时，请使用 `$skip` 分页和 `$top` 查询参数。 有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [accessReviewReviewer](../resources/accessreviewreviewer.md) 对象集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstance_contactedReviewers"
}
-->
``` msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2dca8959-b716-4b4c-a93d-a535c01eb6e0/instances/8d035c9d-798d-47fa-beb4-f986a4b8126f/contactedReviewers
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstance-contactedreviewers-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstance-contactedreviewers-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstance-contactedreviewers-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstance-contactedreviewers-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accessreviewinstance-contactedreviewers-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewReviewer)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('2dca8959-b716-4b4c-a93d-a535c01eb6e0')/instances('8d035c9d-798d-47fa-beb4-f986a4b8126f')/contactedReviewers",
    "@odata.count": 1,
    "value": [
        {
            "id": "139166ec-d214-4835-95aa-3c1d89581e51",
            "displayName": "Adele Vance",
            "userPrincipalName": "AdeleV@contoso.com",
            "createdDateTime": "2021-03-09T23:10:28.83Z"
        }
    ]
}
```
