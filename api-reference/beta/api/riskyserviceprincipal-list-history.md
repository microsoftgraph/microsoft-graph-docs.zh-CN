---
title: 列出 (riskyServicePrincipal) 的风险历史记录
description: 获取 riskyServicePrincipal 对象的风险历史记录。
author: ebasseri
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: e05c7babbea8f51f849e574d687ebde88c284d94
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334588"
---
# <a name="list-history-risk-history-of-riskyserviceprincipal"></a>列出 (riskyServicePrincipal) 的风险历史记录
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [riskyServicePrincipal 对象的风险](../resources/riskyServicePrincipal.md) 历史记录。

>**注意：** 使用 riskyServicePrincipal API 需要一个Azure AD Premium P2许可证。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|IdentityRiskyServicePrincipal.Read.All、IdentityRiskyServicePrincipal.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|IdentityRiskyServicePrincipal.Read.All、IdentityRiskyServicePrincipal.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyServicePrincipals/{riskyServicePrincipalId}/history 
```
## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [riskyServicePrincipalHistoryItem](../resources/riskyserviceprincipalhistoryitem.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_riskyserviceprincipalhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/beta/identityProtection/riskyServicePrincipals/{riskyServicePrincipalId}/history
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-riskyserviceprincipalhistoryitem-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-riskyserviceprincipalhistoryitem-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-riskyserviceprincipalhistoryitem-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-riskyserviceprincipalhistoryitem-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/list-riskyserviceprincipalhistoryitem-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.riskyServicePrincipalHistoryItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#riskyServicePrincipalHistoryItem",
  "value": [
    {
       "id": "0fbef39d-9e8c-460b-444e-8ae5abcdffd7",
       "accountEnabled": true,
       "isProcessing": false,
       "riskLastUpdatedDateTime": "2021-10-20T01:14:37.7214159Z",
       "riskState": "atRisk",
       "riskDetail": "none",
       "riskLevel": "high",
       "displayName": "Contoso App",
       "appId": "ede08db0-9492-4a0c-8ae3-8ggg056c5d75",
       "servicePrincipalType": "Application",
       "servicePrincipalId": "0fbef39d-9e8c-777b-860e-8ae5abcdffd7",
       "initiatedBy": null,
       "activity": null
     }
  ]
}
```
