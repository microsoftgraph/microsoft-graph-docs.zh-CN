---
title: 更新 accessReviewInstanceDecisionItem
description: 更新调用用户是审阅者的现有 accessReviewInstanceDecisionItem 对象。
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 68c5bbbee46ad8df64b09700c66d6731c2a51bb1
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468931"
---
# <a name="update-accessreviewinstancedecisionitem"></a>更新 accessReviewInstanceDecisionItem

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新访问决策，称为 [accessReviewInstanceDecisionItems，](../resources/accessreviewinstancedecisionitem.md)用户是审阅者。

>[!NOTE]
>对 **accessReviewInstanceDecisionItem** 进行的任何更新都只能通过调用列为父 [accessReviewInstance](../resources/accessreviewinstance.md)的审阅者的用户进行。

## <a name="permissions"></a>权限
若要调用此 API，需要以下权限之一。 不支持向个人 Microsoft 帐户委派权限。 若要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

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
下表显示接受更新 的属性 `accessReviewInstanceDecisionItem` 。

| 属性     | 类型       | 说明 |
|:-------------|:------------|:------------|
| decision  | String | 被审阅实体的访问决策。 可能的值是 `Approve` `Deny` `NotReviewed` `DontKnow` ：。 必需。  |
|  justification | String | 提供给管理员评价的上下文。 如果 accessReviewScheduleDefinition 上的 justificationRequiredOnApproval 为 True，则必需。  |

## <a name="response"></a>响应
如果成功，此方法返回 响应 `204, NoContent` 代码，无响应正文。

### <a name="request"></a>请求
## <a name="examples"></a>示例

这是一个批准由 表示的用户的访问的示例 `accessReviewInstanceDecisionItem` 。


<!-- {
  "blockType": "request",
  "name": "update_accessReviewInstanceDecisionItem"
}-->
``` http
PATCH https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/70a68410-67f3-4d4c-b946-6989e050be19/decisions/12348410-67f3-4d4c-b946-6989e050be19
Content-Type: application/json
Content-length: 730

{
  "decision": "Approve",
  "justification": "This person is still on my team",
}
```

---


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessReviewInstanceDecisionItem"
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
