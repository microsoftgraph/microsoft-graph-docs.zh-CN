---
title: accessReviewInstance：batchRecordDecisions
description: 可模拟审阅者分批审阅所有 accessReviewInstanceDecisionItems。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e9573dabd24b414b55fc4ec961999c43896fc687
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469727"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a>accessReviewInstance：batchRecordDecisions
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

允许审阅者使用 、或两者成批查看所有 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) `principalId` `resourceId` 对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|AccessReviews.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|Application|AccessReviews.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
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
| decision  | String | 被审阅实体的访问决策。 可取值为：`Approve`、`Deny`、`NotReviewed`、`DontKnow`。 必需。  |
|  justification | String | 提供给管理员评价的上下文。 如果 **justificationRequiredOnApproval** `True` 位于 **accessReviewScheduleDefinition 上，则是必需的**。  |
|principalId|String|如果提供，将在此批处理中检查具有匹配 **principalId** 的所有 **accessReviewInstanceDecisionItems。** 如果未提供，将 **检查所有 principalId。**|
|resourceId|String|如果提供，将在此批处理中检查具有匹配 **resourceId** 的所有 **accessReviewInstanceDecisionItems。** 如果未提供，将 **检查所有 resourceId。**|



## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/pendingAccessReviewInstances/{accessReviewInstanceId}/batchRecordDecisions
Content-Type: application/json
Content-length: 113

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
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
