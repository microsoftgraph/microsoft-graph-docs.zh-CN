---
title: 更新 accessReviewInstanceDecisionItem
description: 更新调用 user 的现有 accessReviewInstanceDecisionItem 对象是的审阅者。
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 2f14ed26169c659354af16963e03e449f246421c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49214367"
---
# <a name="update-accessreviewinstancedecisionitem"></a>更新 accessReviewInstanceDecisionItem

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新用户为其审阅者的访问决策（称为 " [accessReviewInstanceDecisionItems](../resources/accessreviewinstancedecisionitem.md)"）。

>[!NOTE]
>对 **accessReviewInstanceDecisionItem** 所做的任何更新只能通过呼叫作为父 [accessReviewInstance](../resources/accessreviewinstance.md)的审阅者列出的用户来完成。

## <a name="permissions"></a>权限
若要调用此 API，必须有以下权限之一。 不支持对个人 Microsoft 帐户的委派权限。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/pendingAccessReviewInstances/{instance-id}/decisions/{decision-id}
```
## <a name="request-headers"></a>请求标头
| 名称         | 说明 |
|:-------------|:------------|
|Authorization|Bearer {token}。必需。|
| Content-type | application/json. Required. |

## <a name="request-body"></a>请求正文
下表显示了接受更新的属性 `accessReviewInstanceDecisionItem` 。

| 属性     | 类型       | 说明 |
|:-------------|:------------|:------------|
| 权  | String | 正在审阅的实体的访问决定。 可能的值是： `Approve` `Deny` `NotReviewed` `DontKnow` 。 必需。  |
|  合理化 | String | 向管理员提供的审阅的上下文。 如果 justificationRequiredOnApproval 在 accessReviewScheduleDefinition 上为 True，则为必需项。  |

## <a name="response"></a>响应
如果成功，此方法将返回 `204, NoContent` 响应代码，不返回任何响应正文。

### <a name="request"></a>请求
## <a name="examples"></a>示例

下面的示例展示了如何为由获取的用户审批访问 `accessReviewInstanceDecisionItem` 。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/654b34e7-b48f-4772-a2d4-08f1d0dd014c

{
  "decision": "Approve",
  "justification": "I trust this person"
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

---


---

### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": false
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
