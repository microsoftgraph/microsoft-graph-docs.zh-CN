---
title: 列出 signIn
doc_type: apiPageType
description: 获取租户租户中的用户登录Azure Active Directory列表。
ms.localizationpriority: medium
author: besiler
ms.prod: identity-and-access-reports
ms.openlocfilehash: 6aaf95669860d39ca7d26e1bae2301560e2041c8
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2022
ms.locfileid: "63757771"
---
# <a name="list-signins"></a>列出 signIn

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取 [signIn 对象](../resources/signin.md) 的列表。 该列表包含你的租户的用户Azure Active Directory登录。 用户名和密码作为授权令牌的一部分传递的登录，并且成功的联合登录当前包含在登录日志中。

最大和默认页面大小为 1，000 个对象，默认情况下，首先返回最新的登录。 只有默认保留期Azure Active Directory (Azure AD) [登录事件](/azure/active-directory/reports-monitoring/reference-reports-data-retention#how-long-does-azure-ad-store-the-data)可用。

## <a name="permissions"></a>Permissions

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型 | 权限（从最低特权到最高特权） |
|:--------------- |:------------------------------------------- |
| 委派（工作或学校帐户） | AuditLog.Read.All 和 Directory.Read.All |
| 委派（个人 Microsoft 帐户） | 不支持 |
| 应用程序 | AuditLog.Read.All 和 Directory.Read.All | 

> [!IMPORTANT]
> 此 API 有 [一个已知](/graph/known-issues#license-check-errors-for-azure-ad-activity-reports) 问题，当前需要同意 **AuditLog.Read.All** 和 **Directory.Read.All** 权限。

应用必须[正确注册到](/azure/active-directory/active-directory-reporting-api-prerequisites-azure-portal)Azure AD。

除了委派的权限，登录用户还需要属于以下目录角色之一，以便他们阅读登录报告。 若要了解有关目录角色Azure AD，请参阅Azure AD[角色](/azure/active-directory/roles/permissions-reference)：
+ 全局管理员
+ 全局读取者
+ 报告读取者
+ 安全管理员
+ 安全操作员
+ 安全信息读取者

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
GET auditLogs/signIns
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 、 `$top`和 `$skiptoken``$filter` OData 查询参数来帮助自定义响应。 关如何使用这些参数的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头

| 名称      |说明|
|:----------|:----------|
| Authorization | 持有者 {token} |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [signIn](../resources/signin.md) 对象集合。 对象集合根据 **createdDateTime** 按降序列出。

## <a name="examples"></a>示例

### <a name="example-1-list-all-sign-ins"></a>示例 1：列出所有登录
此示例中，响应对象显示使用由条件访问策略触发的 MFA 登录的用户，并且主要身份验证方法是通过 FIDO。

#### <a name="request"></a>请求

下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signIns
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signins-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-signins-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-signins-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "value": [
    {
      "id":"1691d37b-8579-43a7-966a-0f35583c1300",
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
      "ipAddress":"131.107.159.37",
      "clientAppUsed":"Browser",
      "userAgent":"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36 Edg/91.0.864.54",
      "correlationId":"5d295068-919b-4017-85d8-44be2f5f5483",
      "conditionalAccessStatus":"notApplied",
      "originalRequestId":"7dccb0d7-1041-4d82-b785-d865272e1400",
      "authenticationProtocol": "oAuth2",
      "incomingTokenType": "Primary Refresh Token",
      "isInteractive":true,
      "homeTenantId": "4f7a7bc2-28e2-46a3-b90e-5ade5bc90138",
      "homeTenantName": "",
      "isTenantRestricted": false,
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
      "resourceTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
      "homeTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
      "authenticationMethodsUsed":[],
      "authenticationRequirement":"singleFactorAuthentication",
      "azureResourceId": "/subscriptions/xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx/resourceGroups/testRG/providers/Microsoft.Compute/virtualMachines/testVM",
      "federatedCredentialId": "729ab02a-edd5-4ef5-a285-2d91a3c772ab",
      "uniqueTokenIdentifier": "ZTE0OTk3YTQtZjg5Mi00YjBiLWIwNTEtZmViZTA1YzJhNDli",
      "signInIdentifier":"testaccount1@contoso.com",
      "signInEventTypes":["interactiveUser"],
      "servicePrincipalId":"",
      "sessionLifetimePolicies": [
        {
          "expirationRequirement": "tenantTokenLifetimePolicy",
          "detail": "The user was required to sign in again according to the tenant session lifetime policy"
        }
      ],
      "uniqueTokenIdentifier": "ZTE0OTk3YTQtZjg5Mi00YjBiLWIwNTEtZmViZTA1YzJhNDli",
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
  ]
}
```

### <a name="example-2-retrieve-the-first-10-sign-ins-to-apps-with-the-appdisplayname-that-starts-with-azure"></a>示例 2：检索 appDisplayName 以"Azure"开头的应用的前 10 个登录

此示例中，响应对象显示用户仅使用其主身份验证方法（云密码）登录。 该响应包含 `@odata.nextLink` 一个属性，其中包含可用于检索接下来的 10 个结果的 URL。

#### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_2"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signins?&$filter=startsWith(appDisplayName,'Azure')&top=10
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signins-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-signins-2-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-signins-2-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
  "@odata.nextLink": "https://graph.microsoft.com/beta/auditLogs/signins?$filter=startsWith(appDisplayName%2c%27Azure%27)&$top=10&$skiptoken=3cff228c89605cc89b0dc753668deef4153e8644caa6d83ed1bb5f711b21cba4",
  "value": [
    {
      "id":"1691d37b-8579-43a7-966a-0f35583c1300",
      "createdDateTime":"2021-06-30T16:34:32Z",
      "userDisplayName":"Test contoso",
      "userPrincipalName":"testaccount1@contoso.com",
      "userId":"26be570a-1111-5555-b4e2-a37c6808512d",
      "appId":"c44b4083-3bb0-49c1-b47d-974e53cbdf3c",
      "appDisplayName":"Azure Portal",
      "ipAddress":"131.107.159.37",
      "clientAppUsed":"Browser",
      "userAgent":"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/91.0.4472.114 Safari/537.36 Edg/91.0.864.54",
      "correlationId":"5d295068-919b-4017-85d8-44be2f5f5483",
      "conditionalAccessStatus":"notApplied",
      "homeTenantId": "4f7a7bc2-28e2-46a3-b90e-5ade5bc90138",
      "homeTenantName": "",
      "isTenantRestricted": false,
      "originalRequestId":"7dccb0d7-1041-4d82-b785-d865272e1400",
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
      "resourceTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
      "homeTenantId":"99081087-73c4-48d1-a112-f60ff75114f7",
      "authenticationMethodsUsed":[],
      "authenticationRequirement":"singleFactorAuthentication",
      "authenticationProtocol": "oAuth2",
      "incomingTokenType": "Primary Refresh Token",
      "signInIdentifier":"testaccount1@contoso.com",
      "signInEventTypes":["interactiveUser"],
      "servicePrincipalId":"",
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
      "uniqueTokenIdentifier": "ZTE0OTk3YTQtZjg5Mi00YjBiLWIwNTEtZmViZTA1YzJhNDli",
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
  ]
}
```



### <a name="example-3-retrieve-the-first-10-sign-ins-where-the-signineventtype-is-not-interactiveuser-starting-with-the-latest-sign-in"></a>示例 3：检索 signInEventType 不是交互式用户（从最新登录开始）前 10 个登录

此示例中，响应包含 `@odata.nextLink` 一个属性，其中包含可用于检索接下来的 10 个结果的 URL。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_signins_ne_nonInteractiveUser"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/auditLogs/signins?&$filter=(signInEventTypes/any(t: t ne 'interactiveUser'))&$orderBy=createdDateTime DESC&$top=10
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-signins-ne-noninteractiveuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-signins-ne-noninteractiveuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-signins-ne-noninteractiveuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-signins-ne-noninteractiveuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-signins-ne-noninteractiveuser-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-signins-ne-noninteractiveuser-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a>响应
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#auditLogs/signIns",
    "@odata.nextLink": "https://graph.microsoft.com/beta/auditLogs/signins?$filter=(signInEventTypes%2fany(t%3a+t+ne+%27interactiveUser%27))&$top=10&$orderBy=createdDateTime+DESC&$skiptoken=186ac5626b89ae2a991ff26b674ac381be50b941a40542cb66f8136f2887275b",
    "value": [
        {
            "id": "ef1e1fcc-80bd-489b-82c5-16ad80770e00",
            "createdDateTime": "2022-03-18T18:13:37Z",
            "userDisplayName": "MOD Administrator",
            "userPrincipalName": "admin@contoso.com",
            "userId": "4562bcc8-c436-4f95-b7c0-4f8ce89dca5e",
            "appId": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "appDisplayName": "Graph Explorer",
            "ipAddress": "197.178.9.154",
            "ipAddressFromResourceProvider": null,
            "clientAppUsed": "Browser",
            "userAgent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/99.0.4844.51 Safari/537.36",
            "correlationId": "17b4f05d-3659-42b8-856d-99322911d398",
            "conditionalAccessStatus": "notApplied",
            "originalRequestId": "",
            "isInteractive": false,
            "tokenIssuerName": "",
            "tokenIssuerType": "AzureAD",
            "processingTimeInMilliseconds": 132,
            "riskDetail": "none",
            "riskLevelAggregated": "none",
            "riskLevelDuringSignIn": "none",
            "riskState": "none",
            "riskEventTypes_v2": [],
            "resourceDisplayName": "Microsoft Graph",
            "resourceId": "00000003-0000-0000-c000-000000000000",
            "resourceTenantId": "84841066-274d-4ec0-a5c1-276be684bdd3",
            "homeTenantId": "84841066-274d-4ec0-a5c1-276be684bdd3",
            "homeTenantName": "",
            "authenticationMethodsUsed": [],
            "authenticationRequirement": "singleFactorAuthentication",
            "signInIdentifier": "",
            "signInIdentifierType": null,
            "servicePrincipalName": "",
            "signInEventTypes": [
                "nonInteractiveUser"
            ],
            "servicePrincipalId": "",
            "federatedCredentialId": "",
            "userType": "member",
            "flaggedForReview": false,
            "isTenantRestricted": false,
            "autonomousSystemNumber": 33771,
            "crossTenantAccessType": "none",
            "servicePrincipalCredentialKeyId": "",
            "servicePrincipalCredentialThumbprint": "",
            "uniqueTokenIdentifier": "ZWYxZTFmY2MtODBiZC00ODliLTgyYzUtMTZhZDgwNzcwZTAw",
            "incomingTokenType": "none",
            "authenticationProtocol": "none",
            "resourceServicePrincipalId": "943603e4-e787-4fe9-93d1-e30f749aae39",
            "mfaDetail": null,
            "status": {
                "errorCode": 0,
                "failureReason": "Other.",
                "additionalDetails": null
            },
            "deviceDetail": {
                "deviceId": "eab73519-780d-4d43-be6d-a4a89af2a348",
                "displayName": "DESKTOP-LK3PESR",
                "operatingSystem": "Windows 10",
                "browser": "Chrome 99.0.4844",
                "isCompliant": false,
                "isManaged": false,
                "trustType": "Azure AD registered"
            },
            "location": {
                "city": "Mombasa",
                "state": "Coast",
                "countryOrRegion": "KE",
                "geoCoordinates": {}
            },
            "appliedConditionalAccessPolicies": [
                {
                    "id": "80290cf6-04c8-4a25-8252-2b4d7d88228a",
                    "displayName": "Exchange Online Requires Compliant Device",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none",
                    "includeRulesSatisfied": [],
                    "excludeRulesSatisfied": []
                },
                {
                    "id": "a00746d4-8c33-47f7-b120-91936b367a54",
                    "displayName": "Office 365 App Control",
                    "enforcedGrantControls": [],
                    "enforcedSessionControls": [],
                    "result": "notEnabled",
                    "conditionsSatisfied": "none",
                    "conditionsNotSatisfied": "none",
                    "includeRulesSatisfied": [],
                    "excludeRulesSatisfied": []
                }
            ],
            "authenticationProcessingDetails": [
                {
                    "key": "Root Key Type",
                    "value": "Unknown"
                },
                {
                    "key": "Oauth Scope Info",
                    "value": "[\"Application.ReadWrite.All\",\"AppRoleAssignment.ReadWrite.All\",\"DelegatedPermissionGrant.ReadWrite.All\",\"Directory.ReadWrite.All\",\"openid\",\"profile\",\"RoleManagement.Read.Directory\",\"User.Read\",\"email\",\"AuditLog.Read.All\"]"
                }
            ],
            "networkLocationDetails": [
                {
                    "networkType": "namedNetwork",
                    "networkNames": [
                        "Suspicious countries"
                    ]
                }
            ],
            "authenticationDetails": [],
            "authenticationRequirementPolicies": [],
            "sessionLifetimePolicies": [],
            "privateLinkDetails": {
                "policyId": "",
                "policyName": "",
                "resourceId": "",
                "policyTenantId": ""
            }
        }
    ]
}
```
