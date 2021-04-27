---
title: 列出 accessReviewInstanceDecisionItem
description: 检索 accessReviewInstanceDecisionItem 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7674a129b118c2c9d8c3487623cf039b2ceca603
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048398"
---
# <a name="list-accessreviewinstancedecisionitem"></a>列出 accessReviewInstanceDecisionItem

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

检索 [特定 accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的 [AccessReviewInstance](../resources/accessreviewinstance.md)。 返回零个或多个 accessReviewInstanceDecisionItem 对象的列表，包括其所有嵌套属性。

>[!NOTE]
>如果返回了许多 **accessReviewInstanceDecisionItems，** 为了提高效率并避免超时，请检索页面中的 结果集，方法为在请求中同时包括页面大小最多为 100 的 $top 查询参数和 $skip=0 查询参数。 当结果集跨多个页面时，Microsoft Graph 在响应中返回包含指向下一页结果的 URL 的 @odata.nextLink 属性的页面。 如果存在该属性，请继续在每个响应中通过 @odata.nextLink URL 提出其他请求，直到返回所有结果，如在应用中分页 Microsoft Graph 数据中所述。
>
>如果未提供查询参数且结果超过 100 个，Microsoft Graph将按每页 100 个结果自动对结果分页。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.Read.All、AccessReview.ReadWrite.All  |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序                            | AccessReview.Read.All、AccessReview.ReadWrite.All |

 登录用户还必须具有允许其读取访问评审的目录角色。

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET /identityGovernance/accessReviews/definitions/{definition-id}/instances/{instance-id}/decisions
```
## <a name="request-headers"></a>请求标头
无。

## <a name="request-body"></a>请求正文
不提供请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessReviewInstanceDecisionItem](../resources/accessreviewinstance.md) 对象数组。

## <a name="examples"></a>示例
### <a name="request"></a>请求
以下示例显示检索有关访问评审实例的所有决策的请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_accessReviewInstanceDecisionItem"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/60860cdd-fb4d-4054-91ba-444404f3baa6/instances/14444cdb-6a18-4c08-ba2c-48c02f0a0138/decisions?$top=100&$skip=0
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-accessreviewinstancedecisionitem-java-snippets.md)]
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
    "@odata.count": 4,
    "value": [
        {
            "id": "77a61af9-3bef-4bbf-b00b-04734d6d5eae",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": null,
            "decision": "NotReviewed",
            "justification": "",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
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
                "userId": "3736c87b-dc21-4290-8802-d6fef5fa3a08",
                "userDisplayName": "Irvin Sayers",
                "userPrincipalName": "IrvinS@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "f30b68ef-b843-4479-86b8-0a3a2f4bb209",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:08.377Z",
            "decision": "Approve",
            "justification": "This employee needs access for reason X",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
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
                "userId": "ecd78419-3f1e-4f07-9bd9-7c77137af4f1",
                "userDisplayName": "Bianca Pisani",
                "userPrincipalName": "BiancaP@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "037b737f-e8ca-4507-b126-5a0620ba2c18",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:28.473Z",
            "decision": "Deny",
            "justification": "This employee changed roles and no longer needs access",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
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
                "userId": "5f16b75b-031c-4944-9691-070f03273079",
                "userDisplayName": "Delia Dennis",
                "userPrincipalName": "DeliaD@M365x471116.OnMicrosoft.com"
            }
        },
        {
            "id": "7032f455-10a3-4d04-bf02-66fb65d26d10",
            "accessReviewId": "70463350-742e-4909-bfa5-bc23447bd002",
            "reviewedDateTime": "2020-09-18T16:56:44.38Z",
            "decision": "DontKnow",
            "justification": "I do not know what this employee needs",
            "appliedDateTime": null,
            "applyResult": "New",
            "recommendation": "Deny",
            "reviewedBy": {
                "id": "957f1027-c0ee-460d-9269-b8828e59e0fe",
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
                "userId": "4169762e-895f-4350-a13d-e5b09b1efcfa",
                "userDisplayName": "Isaiah Langer",
                "userPrincipalName": "IsaiahL@M365x471116.OnMicrosoft.com"
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
  "description": "List accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
