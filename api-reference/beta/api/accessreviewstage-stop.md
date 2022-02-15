---
title: accessReviewStage：stop
description: 停止进行中的访问评审阶段。
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 977f46ff45ec63c1b2ca1e932a8fd8df119faa03
ms.sourcegitcommit: 2dd01b49fbd8f330bead92f4708ed1966237c3f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2022
ms.locfileid: "62816136"
---
# <a name="accessreviewstage-stop"></a>accessReviewStage：stop
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

停止 [为 的访问](../resources/accessReviewStage.md) 评审阶段 `inProgress`。 访问评审阶段停止后，**阶段状态将为**`Completed`，审阅者无法再提供输入。 如果存在依赖于已完成阶段的后续阶段，将创建下一个阶段。 

无论阶段的状态如何， [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象将始终反映在给定时间在所有阶段记录的最后决策。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型                        | 权限（从最低特权到最高特权）              |
|:--------------------------------------|:---------------------------------------------------------|
|委派（工作或学校帐户）     | AccessReview.ReadWrite.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序                            | AccessReview.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/stages/{accessReviewStageId}/stop
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "accessreviewstage_stop"
}
-->
``` http
POST https://graph.microsoft.com/beta/identityGovernance/accessReviews/definitions/2b83cc42-09db-46f6-8c6e-16fec466a82d/instances/61a617dd-238f-4037-8fa5-d800e515f5bc/stages/5d431f4b-56f2-4a50-938b-fb1e4e2c91b9/stop
```


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

