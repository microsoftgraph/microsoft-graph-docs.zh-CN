---
title: 获取 accessReviewInstanceDecisionItem
description: 读取 accessReviewInstanceDecisionItem 对象的属性和关系。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 5884841a3e169f0640fe09adb8237bf64816e497
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2022
ms.locfileid: "62815886"
---
# <a name="get-accessreviewinstancedecisionitem"></a>获取 accessReviewInstanceDecisionItem
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

读取 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的属性和关系。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|AccessReview.Read.All、AccessReview.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|AccessReview.Read.All、AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

若要检索对 accessReviewInstance 的决定，
<!-- {
  "blockType": "ignored"
}
-->
```http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

若要从 accessReviewInstance 的阶段检索决策：

<!-- {
  "blockType": "ignored"
}
-->
```http
GET /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/{accessReviewStageId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 OData `$select` 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象。

## <a name="examples"></a>示例

### <a name="example-1-retrieve-a-decision-on-an-accessreviewinstance"></a>示例 1：检索有关 accessReviewInstance 的决定

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-accessreviewinstancedecisionitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identityGovernance/accessReviews/definitions('5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0')/instances('6444d4fd-ab55-4608-8cf9-c6702d172bcc')/decisions/$entity",
    "id": "e6cafba0-cbf0-4748-8868-0810c7f4cc06",
    "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
    "reviewedDateTime": null,
    "decision": "NotReviewed",
    "justification": "",
    "appliedDateTime": null,
    "applyResult": "New",
    "recommendation": "Approve",
    "principalLink": "https://graph.microsoft.com/v1.0/users/04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
    "resourceLink": null,
    "resource": null,
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
        "userId": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
        "userDisplayName": "Diego Siciliani",
        "userPrincipalName": "DiegoS@contoso.com"
    },
    "principal": {
        "@odata.type": "#microsoft.graph.userIdentity",
        "id": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
        "displayName": "Diego Siciliani",
        "userPrincipalName": "DiegoS@contoso.com"
    }
}
```

### <a name="example-2-retrieve-a-decision-from-a-stage-of-a-multi-stage-access-review"></a>示例 2：从多阶段访问评审的阶段检索决策

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_accessreviewstage_accessreviewinstancedecisionitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/stages/9458f255-dff2-4d86-9a05-69438f49d7f8/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06
```

#### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/stages/9458f255-dff2-4d86-9a05-69438f49d7f8/decisions/$entity",
    "id": "e6cafba0-cbf0-4748-8868-0810c7f4cc06",
    "accessReviewId": "6444d4fd-ab55-4608-8cf9-c6702d172bcc",
    "reviewedDateTime": null,
    "decision": "NotReviewed",
    "justification": "",
    "appliedDateTime": null,
    "applyResult": "New",
    "recommendation": "Approve",
    "principalLink": "https://graph.microsoft.com/v1.0/users/04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
    "resourceLink": null,
    "resource": null,
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
        "userId": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
        "userDisplayName": "Diego Siciliani",
        "userPrincipalName": "DiegoS@contoso.com"
    },
    "principal": {
        "@odata.type": "#microsoft.graph.userIdentity",
        "id": "04777c4b-4d43-4d32-a2e7-1eba5d03f8cf",
        "displayName": "Diego Siciliani",
        "userPrincipalName": "DiegoS@contoso.com"
    }
}
```
