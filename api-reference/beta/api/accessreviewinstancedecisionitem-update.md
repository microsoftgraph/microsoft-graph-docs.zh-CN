---
title: 更新 accessReviewInstanceDecisionItem
description: 更新调用用户为审阅者的现有 accessReviewInstanceDecisionItem 对象。
ms.localizationpriority: medium
author: zhusijia26
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e0cf1034cbf8e1a8fbfcfd5d73568431a2ca75de
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697118"
---
# <a name="update-accessreviewinstancedecisionitem"></a>更新 accessReviewInstanceDecisionItem

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新访问决策（称为 [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md)），用户是其审阅者。

>[!NOTE]
>对 **accessReviewInstanceDecisionItem** 所做的任何更新只能通过调用作为父 [accessReviewInstance](../resources/accessreviewinstance.md) 审阅者列出的用户进行。

## <a name="permissions"></a>权限
调用此 API 需要以下权限之一。 不支持向个人 Microsoft 帐户委派权限。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|

## <a name="http-request"></a>HTTP 请求

若要更新 accessReviewInstance 的决策，请执行以下操作：
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

若要更新对具有多个阶段的 accessReviewInstance 阶段的决策：
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/{accessReviewStageId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="request-headers"></a>请求标头
| 名称         | 说明 |
|:-------------|:------------|
| Authorization|Bearer {token}。必需。|
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文
下表显示了接受更新的 `accessReviewInstanceDecisionItem`属性。

| 属性     | 类型       | 说明 |
|:-------------|:------------|:------------|
| 决定  | String | 要审查的实体的访问决策。 可能的值为： `Approve` `NotReviewed` `Deny` `DontKnow`. 必填。  |
|  理由 | String | 提供给管理员的评审的上下文。 如果 accessReviewScheduleDefinition 上的 justificationRequiredOnApproval 为 True，则为必需。  |

## <a name="response"></a>响应
如果成功，此方法将返回响应代码，而不返回 `204 No Content` 响应正文。


## <a name="examples"></a>示例

### <a name="example-1-update-a-decision-on-an-accessreviewinstance"></a>示例 1：更新 accessReviewInstance 的决策

#### <a name="request"></a>请求

下面是决定批准用户访问权限的示例。



# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/stages/9458f255-dff2-4d86-9a05-69438f49d7f8/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06
Content-Type: application/json

{
  "decision": "Approve",
  "justification": "This person is still on my team",
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-accessreviewinstancedecisionitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-accessreviewinstancedecisionitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-accessreviewinstancedecisionitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-accessreviewinstancedecisionitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-accessreviewinstancedecisionitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 Accepted
```


### <a name="example-2-update-a-decision-on-an-stage-in-a-multi-stage-access-review"></a>示例 2：在多阶段访问评审中更新有关某个阶段的决策

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
``` http
PATCH https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/5eac5a70-7cd7-4f20-92b0-f9dba70dd7f0/instances/6444d4fd-ab55-4608-8cf9-c6702d172bcc/stages/9458f255-dff2-4d86-9a05-69438f49d7f8/decisions/e6cafba0-cbf0-4748-8868-0810c7f4cc06
Content-Type: application/json

{
  "decision": "Approve",
  "justification": "This person is still on my team",
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 Accepted
```

<!--
{
  "type": "#page.annotation",
  "description": "Update accessReviewInstanceDecisionItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
