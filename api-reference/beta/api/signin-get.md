---
title: 获取 signIn
doc_type: apiPageType
description: 获取一个 signIn 对象，该对象包含Azure Active Directory租户的所有登录。
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: f6880fe40bc4560454b985f00bef03eec7891868
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820733"
---
# <a name="get-signin"></a>获取 signIn

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取一个 [signIn](../resources/signin.md) 对象，该对象包含租户的特定用户登录事件。 这包括要求用户输入用户名或密码的登录，以及会话令牌。

[!INCLUDE [GDPR-related-guidance](../../includes/gdpr-msgraph-export-note.md)]

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
| 委派（工作或学校帐户） | AuditLog.Read.All 和 Directory.Read.All |
| 委派（个人 Microsoft 帐户） | 不支持 |
| 应用程序 | AuditLog.Read.All 和 Directory.Read.All | 

> [!IMPORTANT]
> 此 API 存在 [已知问题](/graph/known-issues#license-check-errors-for-azure-ad-activity-reports) ，当前需要同意 **AuditLog.Read.All** 和 **Directory.Read.All** 权限。

应用必须 [正确注册](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal) 到 Azure AD。

除了委派的权限外，已登录的用户还需要属于以下目录角色之一，这些角色允许他们读取登录报告。 若要详细了解目录角色，请参阅 [Azure AD 内置角色](/azure/active-directory/roles/permissions-reference)：
+ 全局管理员
+ 全局读取者
+ 报告读取者
+ 安全管理员
+ 安全操作员
+ 安全读取者

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->
```http
GET /auditLogs/signIns/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 OData 查询参数来帮助自定义响应。 关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signin_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns/66ea54eb-blah-4ee5-be62-ff5a759b0100
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signin-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signin-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signin-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signin-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-signin-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-signin-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.signIn"
} -->


```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id":"66ea54eb-blah-4ee5-be62-ff5a759b0100",
  "createdDateTime":"2021-06-30T16:34:32Z",
  "userDisplayName":"Test contoso",
  "userPrincipalName":"testaccount1@contoso.com",
  "userId":"26be570a-1111-5555-b4e2-a37c6808512d",
  "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
  "appDisplayName":"Azure Portal",
  "authenticationContextClassReferences": [
      {
        "id":"C1",
        "details":"required"
      }
  ],
  "authenticationProtocol": "oAuth2",
  "incomingTokenType": "Primary Refresh Token",
  "ipAddress":"131.107.159.37",
  "clientAppUsed":"Browser",
  "clientCredentialType": "certificate",
  "userAgent":"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36 Edg/91.0.864.54",
  "correlationId":"5d295068-919b-4017-85d8-44be2f5f5483",
  "conditionalAccessStatus":"notApplied",
  "originalRequestId":"7dccb0d7-1041-4d82-b785-d865272e1400",
  "homeTenantId": "4f7a7bc2-28e2-46a3-b90e-5ade5bc90138",
  "homeTenantName": "",
  "isTenantRestricted": false,
  "isInteractive":true,
  "tokenIssuerName":"",
  "tokenIssuerType":"AzureAD",
  "processingTimeInMilliseconds":761,
  "riskDetail":"none",
  "riskLevelAggregated":"none",
  "riskLevelDuringSignIn":"none",
  "riskState":"none",
  "riskEventTypes_v2":[],
  "resourceDisplayName":"Windows Azure Service Management API",
  "resourceId":"797f4846-ba00-4fd7-ba43-dac1f8f63013",
  "resourceServicePrincipalId": "a6033f22-27f9-45cb-8f63-7dd8a0590e4e",
  "uniqueTokenIdentifier": "ZTE0OTk3YTQtZjg5Mi00YjBiLWIwNTEtZmViZTA1YzJhNDli",
  "resourceTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
  "homeTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
  "authenticationMethodsUsed":[],
  "authenticationRequirement":"singleFactorAuthentication",
  "azureResourceId": "/subscriptions/xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx/resourceGroups/testRG/providers/Microsoft.Compute/virtualMachines/testVM",
  "federatedCredentialId": "729ab02a-edd5-4ef5-a285-2d91a3c772ab",
  "signInIdentifier":"testaccount1@contoso.com",
  "signInEventTypes":["interactiveUser"],
  "servicePrincipalId":"",
  "sessionLifetimePolicies": [
    {
      "expirationRequirement": "tenantTokenLifetimePolicy",
      "detail": "The user was required to sign in again according to the tenant session lifetime policy"
    }
  ],
  "userType":"member",
  "flaggedForReview":false,
  "isTenantRestricted":false,
  "autonomousSystemNumber":3598,
  "crossTenantAccessType":"none",
  "status":{
      "errorCode":50126,
      "failureReason":"Error validating credentials due to invalid username or password.",
      "additionalDetails":"The user didn't enter the right credentials. \u00a0It's expected to see some number of these errors in your logs due to users making mistakes."
    },
  "deviceDetail":{
      "deviceId":"",
      "displayName":"",
      "operatingSystem":"Windows 10",
      "browser":"Edge 91.0.864",
      "isCompliant":false,
      "isManaged":false,
      "trustType":""
    },
  "location":{
      "city":"Redmond",
      "state":"Washington",
      "countryOrRegion":"US",
      "geoCoordinates":{
        "altitude":null,
        "latitude":47.6807,
        "longitude":-122.1231
      }
    },
  "appliedConditionalAccessPolicies":[],
  "authenticationProcessingDetails":[
      {
        "key":"Login Hint Present",
        "value":"True"
      }
    ],
  "networkLocationDetails":[
      {
        "networkType":"namedNetwork",
        "networkNames":["North America"]
      }
    ],
  "authenticationDetails":[
      {
        "authenticationStepDateTime":"2021-06-30T16:34:32Z",
        "authenticationMethod":"Password",
        "authenticationMethodDetail":"Password in the cloud",
        "succeeded":false,
        "authenticationStepResultDetail":"Invalid username or password or Invalid on-premise username or password.",
        "authenticationStepRequirement":"Primary authentication"
      }
    ],
  "authenticationRequirementPolicies":[],
  "sessionLifetimePolicies":[]
}
```
