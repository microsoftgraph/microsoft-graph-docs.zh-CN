---
title: signIn：confirmSafe
description: 允许管理员将 Azure AD 登录事件标记为 Azure AD 标识保护的安全。
author: besiler
ms.localizationpriority: medium
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: 6cf66686b1261fdf34742c9e710e1f02a3ac12a1
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447239"
---
# <a name="signin-confirmsafe"></a>signIn：confirmSafe
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

允许管理员将 Azure AD 登录日志中的事件标记为安全。 管理员可以将 Azure AD 标识保护标记为有风险的事件标记为安全，也可以将未标记的事件标记为安全。 有关调查标识保护风险的详细信息，请参阅 [如何调查风险](/azure/active-directory/identity-protection/howto-identity-protection-investigate-risk)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|IdentityRiskyUser.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|IdentityRiskEvent.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /auditLogs/signIns/confirmSafe
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
|requestIds|字符串集合|应为 Azure AD 标识保护标记为安全的登录事件的 ID。|



## <a name="response"></a>响应

如果成功，此操作返回 `204 No Content` 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "signinthis.confirmsafe"
}
-->
``` http
POST https://graph.microsoft.com/beta/auditLogs/signIns/confirmSafe
Content-Type: application/json

{
  "requestIds": [
    "5a0c76d2-cb57-4ece-9bc1-c323178f116a",
    "96609214-09ef-4f80-9d4a-ace5fceecaec",
    "05020696-4eb8-45a3-918f-8f8bb7ad6015"
  ]
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/signinthisconfirmsafe-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/signinthisconfirmsafe-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/signinthisconfirmsafe-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/signinthisconfirmsafe-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/signinthisconfirmsafe-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/signinthisconfirmsafe-powershell-snippets.md)]
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

