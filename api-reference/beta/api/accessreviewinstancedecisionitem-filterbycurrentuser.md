---
title: accessReviewInstanceDecisionItem：filterByCurrentUser
description: 检索调用用户是审阅者的 accessReviewInstance 上的所有 accessReviewInstanceDecisionItem 对象。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e34a595bb0f10eb8b1e18ecba03b94348b8807f2
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61223920"
---
# <a name="accessreviewinstancedecisionitem-filterbycurrentuser"></a>accessReviewInstanceDecisionItem：filterByCurrentUser
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索调用用户是审阅者的给定 accessReviewInstance 上的所有[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象。 [](../resources/accessreviewinstance.md)

>[!NOTE]
>此 API 的默认页面大小为 100 accessReviewInstanceDecisionItem 对象。 若要提高效率并避免由于大型结果集而超时，请通过使用 和 查询参数应用 `$skip` `$top` 分页。 有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|AccessReview.Read.All、AccessReview.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|Application|AccessReview.Read.All、AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/filterByCurrentUser(on='reviewer')
```

## <a name="function-parameters"></a>函数参数
下表显示了可用于此方法的查询参数。

|参数|类型|说明|
|:---|:---|:---|
|on|accessReviewInstanceDecisionItemFilterByCurrentUserOptions|筛选以查询当前用户的决策对象。 可能的值是 `reviewer` `unknownFutureValue` 、。 使用 `reviewer` 。 必需。|


## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$select` 、 `$filter` `$orderBy` 、 、 `$skip` 和 `$top` OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此函数在响应正文中返回 响应代码和 `200 OK` [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 集合。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstancedecisionitem_filterbycurrentuser"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/0185aab8-9a7e-44b5-ae36-41b923c3bf87/instances/1234aab8-9a7e-5678-ae36-41b923c3bf87/decisions/filterByCurrentUser(on='reviewer')
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstancedecisionitem-filterbycurrentuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstancedecisionitem-filterbycurrentuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstancedecisionitem-filterbycurrentuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstancedecisionitem-filterbycurrentuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accessreviewinstancedecisionitem-filterbycurrentuser-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessReviewInstanceDecisionItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(accessReviewInstanceDecisionItem)",
    "@odata.count": 1,
    "value": [
        {
            "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItem",
            "id": "139166ec-d214-4835-95aa-3c1d89581e51",
            "accessReviewId": "8d035c9d-798d-47fa-beb4-f986a4b8126f",
            "reviewedDateTime": "2021-05-03T19:28:25.02Z",
            "decision": "Approve",
            "justification": "Kathleen still needs access to the Marketing group as she works in the Marketing organization.",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "principalLink": "https://graph.microsoft.com/v1.0/users/1800bb2c-955d-4205-8471-3a6c3116435d",
            "resourceLink": null,
            "resource": null,
            "reviewedBy": {
                "id": "36c4c56e-fce3-4e2d-b28e-4ac0c7d2fa10",
                "displayName": "MOD Administrator",
                "userPrincipalName": "MOD Administrator"
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "userDisplayName": "guest example",
                "userPrincipalName": "guest@guest.com"
            },
            "principal": {
                "@odata.type": "#microsoft.graph.userIdentity",
                "id": "1800bb2c-955d-4205-8471-3a6c3116435d",
                "displayName": "guest example",
                "userPrincipalName": "guest@contoso.com"
            }
        }
    ]
}
```
