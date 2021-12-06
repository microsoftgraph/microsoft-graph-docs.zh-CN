---
title: accessReviewInstance：batchRecordDecisions
description: 使审阅者可以分批审阅所有 accessReviewInstanceDecisionItems。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a01ca2f4525661113ed77f0d9eaf65c731f99b15
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974731"
---
# <a name="accessreviewinstance-batchrecorddecisions"></a>accessReviewInstance：batchRecordDecisions
命名空间：microsoft.graph

允许审阅者使用 **principalId** **、resourceId** 或两者成批查看所有 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)对象。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|AccessReview.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持|
|应用程序|AccessReview.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/batchRecordDecisions
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)的 JSON 表示形式。

下表列出了可用于查看 [accessReviewInstanceDecisionItem 对象](../resources/accessreviewinstancedecisionitem.md) 的属性。

|参数|类型|说明|
|:---|:---|:---|
|decision|String|被审阅实体的访问决策。 可能的值是：`Approve`、`Deny`、`NotReviewed`、`DontKnow`。 必需。|
|justification|String|提供给管理员评价的上下文。 如果 **accessReviewScheduleDefinition** 的 settings 属性的 **justificationRequiredOnApproval** 为 ，则必需 `true` 。|
|principalId|String|如果提供，将在此批处理中检查具有匹配 **principalId** 值的所有 **accessReviewInstanceDecisionItems。** 如果未提供，将检查 **所有 accessReviewInstanceDecisionItems。**|
|resourceId|String|如果提供，将在此批处理中检查具有匹配 **resourceId** 的所有 **accessReviewInstanceDecisionItems。** 如果未提供，将检查 **所有 accessReviewInstanceDecisionItems。**|

## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "accessreviewinstance_batchrecorddecisions"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/e6cafba0-cbf0-4748-8868-0810c7f4cc06/instances/1234fba0-cbf0-6778-8868-9999c7f4cc06/batchRecordDecisions
Content-type: application/json

{
  "decision": "Approve",
  "justification": "All principals with access need continued access to the resource (Marketing Group) as all the principals are on the marketing team",
  "resourceId": "a5c51e59-3fcd-4a37-87a1-835c0c21488a"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/accessreviewinstance-batchrecorddecisions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/accessreviewinstance-batchrecorddecisions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/accessreviewinstance-batchrecorddecisions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/accessreviewinstance-batchrecorddecisions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/accessreviewinstance-batchrecorddecisions-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
