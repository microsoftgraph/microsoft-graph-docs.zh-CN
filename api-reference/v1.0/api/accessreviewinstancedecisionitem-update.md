---
title: 更新 accessReviewInstanceDecisionItem
description: 更新 accessReviewInstanceDecisionItem 对象的属性。
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 0d06d62ddcf5568e451e2309180022fdd1c77717
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59038648"
---
# <a name="update-accessreviewinstancedecisionitem"></a>更新 accessReviewInstanceDecisionItem
命名空间：microsoft.graph

更新 [accessReviewInstanceDecisionItem 对象](../resources/accessreviewinstancedecisionitem.md) 的属性。


## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|AccessReview.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|AccessReview.ReadWrite.All|

只有列为父 [accessReviewInstance](../resources/accessreviewinstance.md) 审阅者的调用用户才能更新 **accessReviewInstanceDecisionItem**。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}/instances/{accessReviewInstanceId}/decisions/{accessReviewInstanceDecisionItemId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) 对象的 JSON 表示形式。

下表显示更新 [accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)时接受的属性。

|属性|类型|说明|
|:---|:---|:---|
|decision|String|审阅者对主体是否应有权访问所审阅的资源的投票。 可能的值 `Approve` ：、 `Deny` 或 `DontKnow` 。 必需。|
|justification|String|审阅者的决策原因。 如果 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)的 settings 属性的 **justificationRequiredOnApproval** 为 ，则必需 `true` 。|

## <a name="response"></a>响应

如果成功，此方法返回 `204 OK` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_accessreviewinstancedecisionitem"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/abadf3b6-8ea4-4dea-90a5-9eac8fe93fbd/instances/4444f3b6-8ea4-4dea-90a5-9eac8fe95678/decisions/5555f3b6-8ea4-4dea-90a5-9eac8fe95555
Content-Type: application/json
Content-length: 691

{
  "decision": "Approve",
  "justification": "Kathleen still needs access to the Marketing group as she works in the Marketing organization."
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



### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
