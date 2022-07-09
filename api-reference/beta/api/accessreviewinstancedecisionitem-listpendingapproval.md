---
title: 列出待审批的 accessReviewInstanceDecisionItem
description: 检索待调用用户批准的 accessReviewInstanceDecisionItem 对象。
ms.localizationpriority: medium
author: zhusijia26
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 85e42de0bffa25377fb6a2eba9332adba6d85b20
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66696602"
---
# <a name="list-accessreviewinstancedecisionitems-pending-approval-deprecated"></a>列出 accessReviewInstanceDecisionItems 挂起审批 (已弃用) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>此方法将被弃用，并将于 2023 年 5 月 19 日停止返回数据。 它已被 [filterByCurrentUser](accessreviewinstancedecisionitem-filterbycurrentuser.md) 替换。

检索某个特定 [accessReviewInstance](../resources/accessreviewscheduledefinition.md) [的 accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) 对象，等待调用用户批准。 返回零个或多个 accessReviewInstanceDecisionItem 对象的列表，包括其所有嵌套属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.Read.All、AccessReview.ReadWrite.All  |
|委派（个人 Microsoft 帐户）|不支持。|

登录用户也只会在该决策的实例的 accessReviewScheduleDefinition 中看到分配了审阅者的决定。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /me/pendingAccessReviewInstances/{instance-id}/decisions
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 `$skip` OData `$top` 查询参数，以帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

此 API 的默认页面大小为 100 **个 accessReviewInstanceDecisionItem** 对象。 若要提高效率并避免因大型结果集而超时，请使用 `$skip` 分页和 `$top` 查询参数。 有关详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。

## <a name="request-headers"></a>请求标头
无。

## <a name="request-body"></a>请求正文
请勿提供请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) 对象数组。

## <a name="examples"></a>示例
### <a name="request"></a>请求
以下示例演示一个请求，请求检索对访问评审实例的所有决策，等待调用用户的批准。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem_pendingapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions?$top=100&$skip=0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-pendingapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-pendingapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-pendingapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-pendingapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-accessreviewinstancedecisionitem-pendingapproval-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem",
  "isCollection": "true"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.count": 2,
    "value": [
        {
            "id": "654b34e7-b48f-4772-a2d4-08f1d0dd014c",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "7eae986b-d425-48b2-adf2-3c777f6256f3",
                "userDisplayName": "Adele Vance",
                "userPrincipalName": "AdeleV@contoso.com"
            }
        },
        {
            "id": "0311dba4-c60c-412e-ac77-14e1da23daf1",
            "accessReviewId": "70a68410-67f3-4d4c-b946-6989e050be19",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Approve",
            "reviewedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "appliedBy": {
                "id": "00000000-0000-0000-0000-000000000000",
                "displayName": "",
                "userPrincipalName": ""
            },
            "target": {
                "@odata.type": "#microsoft.graph.accessReviewInstanceDecisionItemUserTarget",
                "userId": "957f1027-c0ee-460d-9269-b8828e59e0fe",
                "userDisplayName": "MOD Administrator",
                "userPrincipalName": "admin@contoso.com"
            }
        }
    ]
}
```

## <a name="see-also"></a>另请参阅

- [获取 accessReviewScheduleDefinition](accessreviewscheduledefinition-get.md)
- [获取 accessReviewInstance](accessreviewinstance-get.md)


<!--
{
  "type": "#page.annotation",
  "description": "List accessReviewInstanceDecisionItem pendingApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
