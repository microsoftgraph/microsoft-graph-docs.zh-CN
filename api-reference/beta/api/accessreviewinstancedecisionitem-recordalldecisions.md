---
title: accessReviewInstanceDecisionItem：recordAllDecisions
description: 记录 accessReviewInstanceDecisionItem 对象的决策。
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fb5fd711253e15c8609ce7cac16452dae6a6c9c1
ms.sourcegitcommit: 3f3975916b5c531ee63d92340ccd6e73e879e8d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2022
ms.locfileid: "62162189"
---
# <a name="accessreviewinstancedecisionitem-recordalldecisions"></a>accessReviewInstanceDecisionItem：recordAllDecisions
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

作为访问评审的审阅者，记录分配给您的 [accessReviewInstanceDecisionItem](../resources/accessReviewInstanceDecisionItem.md) 与指定的主体或资源 ID 相匹配的决策。 如果未指定任何 ID，则决策将应用于您作为审阅者的每个 **accessReviewInstanceDecisionItem。**

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.Read.All、AccessReview.ReadWrite.All  |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序                            | AccessReview.Read.All、AccessReview.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/decisions/filterByCurrentUser(on='reviewer')/recordAllDecisions
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|:---|:---|:---|
|decision|String| 提供的决策。 可能的值为 `Approve` `Deny` `DontKnow` 、、。 |
|justification|String|提供决策的理由。|
|principalId|String|如果提供，与 principalId 匹配的所有决策项都将记录此决策。|
|resourceId|String|如果提供，将记录与 resourceId 匹配的所有决策项。|



## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "accessreviewinstancedecisionitem-recordalldecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/decisions/filterByCurrentUser(on='reviewer')/recordAllDecisions
Content-Type: application/json

{
  "decision": "Deny",
  "justification": "Alice switched teams and no longer works with this group",
  "principalId": "2043848d-e422-473c-8607-88a3319ff491",
  "resourceId": "733ef921-89e1-4d7e-aeff-83612223c37e"
}
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

