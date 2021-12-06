---
title: 更新 adminConsentRequestPolicy
description: 更新 adminConsentRequestPolicy 对象的属性。
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2cc16ba867e5084814565201d8ad8d056fd1dc37
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996811"
---
# <a name="update-adminconsentrequestpolicy"></a>更新 adminConsentRequestPolicy

命名空间：microsoft.graph

更新 [adminConsentRequestPolicy 对象](../resources/adminconsentrequestpolicy.md) 的属性。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|Policy.ReadWrite.ConsentRequest、Directory.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|Policy.ReadWrite.ConsentRequest、Directory.ReadWrite.All|

代表用户进行呼叫时，用户需要属于全局 [管理员](/azure/active-directory/roles/permissions-reference) 目录角色。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PUT /policies/adminConsentRequestPolicy
```

## <a name="request-headers"></a>请求标头

|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

在请求正文中，提供 [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 对象的 JSON 表示形式。

下表显示更新 [adminConsentRequestPolicy 时所需的属性](../resources/adminconsentrequestpolicy.md)。

|属性|类型|说明|
|:---|:---|:---|
|isEnabled|Boolean|指定是启用还是禁用管理员同意请求功能。|
|notifyReviewers|布尔|指定审阅者是否将收到通知。|
|remindersEnabled|布尔|指定审阅者是否将收到提醒电子邮件。|
|requestDurationInDays|Int32|指定请求在未应用决策时自动过期之前处于活动状态的持续时间。|
|reviewers|[accessReviewReviewerScope](../resources/accessreviewreviewerscope.md) 集合|管理员同意的审阅者列表。|

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 响应代码和更新的 `204 No content` [adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_adminconsentrequestpolicy"
}
-->
``` http
PUT https://graph.microsoft.com/v1.0/policies/adminConsentRequestPolicy 
Content-Type: application/json

{
  "isEnabled": true,
  "notifyReviewers": true,
  "remindersEnabled": true,
  "requestDurationInDays": 5,
  "reviewers": [
    {
      "query": "/users/b6879be8-fb87-4482-a72e-18445d2b5c54",
      "queryType": "MicrosoftGraph"
    },
    {
      "query": "/users/b3427cc5-bf69-4dcd-95f7-ed1eb432f5e9",
      "queryType": "MicrosoftGraph"
    }
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-adminconsentrequestpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-adminconsentrequestpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-adminconsentrequestpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-adminconsentrequestpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-adminconsentrequestpolicy-go-snippets.md)]
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
Content-Type: text/plain
```
