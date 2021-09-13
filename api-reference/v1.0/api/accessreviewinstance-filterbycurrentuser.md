---
title: accessReviewInstance：filterByCurrentUser
description: 检索给定审阅者的所有 accessReviewInstance 对象。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4725764f31252568ce1946cbcdbd5c95797a6381
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59033096"
---
# <a name="accessreviewinstance-filterbycurrentuser"></a>accessReviewInstance：filterByCurrentUser
命名空间：microsoft.graph

检索给定[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)上的所有[accessReviewInstance](../resources/accessreviewinstance.md)对象，其中调用用户是一个或多个[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象的审阅者。

>[!NOTE]
>此 API 的默认页面大小为 100 accessReviewInstance 对象。 若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。 有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|AccessReview.Read.All、AccessReview.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|AccessReview.Read.All、AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/filterByCurrentUser(on='reviewer')
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select` 、 、 、 和 OData 查询参数 `$filter` `$orderBy` `$skip` `$top` 来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [accessReviewInstance](../resources/accessreviewinstance.md) 集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/filterByCurrentUser(on='reviewer')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(accessReviewInstance)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstance",
            "id": "7ca879f0-77ea-4386-b110-776dec898935",
            "startDateTime": "2021-04-20T00:45:51.627Z",
            "endDateTime": "2021-04-23T00:45:51.627Z",
            "status": "Applied",
            "scope": {
                "@odata.type": "#microsoft.graph.accessReviewQueryScope",
                "query": "/v1.0/groups/6b7b9930-38a0-4f93-a107-3bc9904c83d7/members/microsoft.graph.user/?$count=true&$filter=(userType eq 'Guest')",
                "queryType": "MicrosoftGraph",
                "queryRoot": null
            }
        }
    ]
}
```
