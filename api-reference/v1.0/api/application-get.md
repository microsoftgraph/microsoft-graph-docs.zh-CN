---
title: 获取应用程序
description: 获取 application 对象的属性和关系。
author: sureshja
ms.localizationpriority: high
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 78a23b03c1918aa1badd14cdb4a57a6a00d78413
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668641"
---
# <a name="get-application"></a>获取应用程序

命名空间：microsoft.graph

获取 [application](../resources/application.md) 对象的属性和关系。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | Application.Read.All、Application.ReadWrite.All、Directory.Read.All    |
|委派（个人 Microsoft 帐户） | Application.Read.All， Application.ReadWrite.All |
|应用程序 | Application.Read.All、Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All |

## <a name="http-request"></a>HTTP 请求
将 `{id}` 替换为应用程序对象的 **ID**，在 Azure 门户中也称为 **对象 ID**。
<!-- { "blockType": "ignored" } -->
```http
GET /applications/{id}
```

## <a name="optional-query-parameters"></a>可选的查询参数

此方法支持 `$select` [OData 查询参数](/graph/query-parameters) 检索特定应用程序属性。

默认情况下，此 API 不会返回 **keyCredentials** 属性中 **密钥** 的公钥值，除非已在 `$select` 查询中指定了 **keyCredentials**。例如，`$select=id,appId,keyCredentials`。

对于每个租户，使用 `$select` 获取应用程序的 **keyCredentials** 的限制为每分钟 150 个请求。

## <a name="request-headers"></a>请求标头

| 名称           | 说明                |
|:---------------|:---------------------------|
| Authorization  | Bearer {token}。必需。  |

## <a name="request-body"></a>请求正文

请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [application](../resources/application.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_application"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/{id}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-application-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-application-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-application-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
下面是一个响应示例。 

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications/$entity",
    "id": "03ef14b0-ca33-4840-8f4f-d6e91916010e",
    "deletedDateTime": null,
    "isFallbackPublicClient": null,
    "appId": "631a96bc-a705-4eda-9f99-fdaf9f54f6a2",
    "applicationTemplateId": null,
    "identifierUris": [],
    "createdDateTime": "2019-09-17T19:10:35.2742618Z",
    "disabledByMicrosoftStatus": null,
    "displayName": "Display name",
    "isDeviceOnlyAuthSupported": null,
    "groupMembershipClaims": null,
    "optionalClaims": null,
    "addIns": [],
    "publisherDomain": "contoso.onmicrosoft.com",
    "samlMetadataUrl": "https://graph.microsoft.com/2h5hjaj542de/app",
    "signInAudience": "AzureADandPersonalMicrosoftAccount",
    "verifiedPublisher": {
            "displayName": "publisher_contoso",
            "verifiedPublisherId": "9999999",
             "addedDateTime": "2021-04-24T17:49:44Z"
    },
    "certification": {
           "isPublisherAttested": true,
           "isCertifiedByMicrosoft": true,
           "lastCertificationDateTime": "2021-05-11T23:26:20Z",
           "certificationExpirationDateTime": "2022-05-11T23:26:20Z",
           "certificationDetailsUrl": "https://docs.microsoft.com/microsoft-365-app-certification/forward/azure/631a96bc-a705-4eda-9f99-fdaf9f54f6a2"
    },
    "tags": [],
    "tokenEncryptionKeyId": null,
    "api": {
        "requestedAccessTokenVersion": 2,
        "acceptMappedClaims": null,
        "knownClientApplications": [],
        "oauth2PermissionScopes": [],
        "preAuthorizedApplications": []
    },
    "appRoles": [],
    "publicClient": {
        "redirectUris": []
    },
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "parentalControlSettings": {
        "countriesBlockedForMinors": [],
        "legalAgeGroupRule": "Allow"
    },
    "passwordCredentials": [],
    "requiredResourceAccess": [],
    "web": {
        "redirectUris": [],
        "homePageUrl": null,
        "logoutUrl": null,
        "implicitGrantSettings": {
            "enableIdTokenIssuance": false,
            "enableAccessTokenIssuance": false
        }
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

