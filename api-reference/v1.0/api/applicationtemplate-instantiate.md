---
title: applicationTemplate：实例化
description: 将应用程序的实例从Azure AD应用程序库添加到目录中。
ms.localizationpriority: medium
author: luleonpla
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 83fa2386e3e083dd515bf8e53f7afe0ada97061c
ms.sourcegitcommit: 5516b107d72caef6ec042fe74228be4031b32fa5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2022
ms.locfileid: "65059912"
---
# <a name="applicationtemplate-instantiate"></a>applicationTemplate：实例化

命名空间：microsoft.graph

将应用程序的实例从Azure AD应用程序库添加到目录中。 还可以使用此 API 实例化 [非库应用](/azure/active-directory/manage-apps/add-non-gallery-app)。 对 **applicationTemplate** 对象使用以下 ID： `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`.

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权）        |
| :------------------------------------- | :------------------------------------------------- |
| 委派（工作或学校帐户）     | Application.ReadWrite.All、Directory.ReadWrite.All |
| 委派（个人 Microsoft 帐户） | 不支持。                                     |
| 应用程序                            | Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
POST /applicationTemplates/{applicationTemplate-id}/instantiate
```

若要实例化非库应用，请使用`8adf8e6e-67b2-4cf2-a259-e3dc5476c621` `{applicationTemplate-id}`

## <a name="request-headers"></a>请求标头

| 名称          | 说明   |
| :------------ | :------------ |
| Authorization | Bearer {code} |

## <a name="request-body"></a>请求正文

在请求正文中，提供具有以下参数的 JSON 对象。

| 参数   | 类型   | 说明                    |
| :---------- | :----- | :----------------------------- |
| displayName | String | 应用程序的自定义名称 |

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `201 Created` 响应代码和新的 [applicationServicePrincipal](../resources/applicationserviceprincipal.md) 对象。

## <a name="examples"></a>示例

以下示例演示如何调用此 API。

### <a name="request"></a>请求

下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```http
POST https://graph.microsoft.com/v1.0/applicationTemplates/229946b9-a9fb-45b8-9531-efa47453ac9e/instantiate
Content-type: application/json

{
    "displayName": "Azure AD SAML Toolkit"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/applicationtemplate-instantiate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/applicationtemplate-instantiate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/applicationtemplate-instantiate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/applicationtemplate-instantiate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/applicationtemplate-instantiate-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/applicationtemplate-instantiate-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应

下面展示了示例响应。

> **注意：** 为了提高可读性，可能缩短了此处显示的响应对象。 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.applicationServicePrincipal",
    "application": {
        "id": "20845737-a145-446f-aa3c-77d432903957",
        "appId": "3c653ec4-4e4c-4820-8127-49e3889cad99",
        "applicationTemplateId": "229946b9-a9fb-45b8-9531-efa47453ac9e",
        "createdDateTime": "2022-04-25T16:48:24Z",
        "deletedDateTime": null,
        "displayName": "Azure AD SAML Toolkit",
        "groupMembershipClaims": null,
        "identifierUris": [],
        "isFallbackPublicClient": false,
        "signInAudience": "AzureADMyOrg",
        "tags": [],
        "tokenEncryptionKeyId": null,
        "defaultRedirectUri": null,
        "optionalClaims": null,
        "addIns": [],
        "api": {
            "acceptMappedClaims": null,
            "knownClientApplications": [],
            "requestedAccessTokenVersion": null,
            "oauth2PermissionScopes": [
                {
                    "adminConsentDescription": "Allow the application to access Azure AD SAML Toolkit on behalf of the signed-in user.",
                    "adminConsentDisplayName": "Access Azure AD SAML Toolkit",
                    "id": "00e7ef81-4deb-41d7-9ee3-90d4eba1e991",
                    "isEnabled": true,
                    "type": "User",
                    "userConsentDescription": "Allow the application to access Azure AD SAML Toolkit on your behalf.",
                    "userConsentDisplayName": "Access Azure AD SAML Toolkit",
                    "value": "user_impersonation"
                }
            ],
            "preAuthorizedApplications": []
        },
        "appRoles": [
            {
                "allowedMemberTypes": [
                    "User"
                ],
                "displayName": "msiam_access",
                "id": "8b292bda-39b6-4b77-849e-887565235bb0",
                "isEnabled": true,
                "description": "msiam_access",
                "value": null,
                "origin": "Application"
            }
        ],
        "info": {
            "logoUrl": null,
            "marketingUrl": null,
            "privacyStatementUrl": null,
            "supportUrl": null,
            "termsOfServiceUrl": null
        },
        "keyCredentials": [],
        "parentalControlSettings": {
            "countriesBlockedForMinors": [],
            "legalAgeGroupRule": "Allow"
        },
        "passwordCredentials": [],
        "publicClient": {
            "redirectUris": []
        },
        "requiredResourceAccess": [],
        "verifiedPublisher": {
            "displayName": null,
            "verifiedPublisherId": null,
            "addedDateTime": null
        },
        "web": {
            "homePageUrl": "https://samltoolkit.azurewebsites.net/SAML/Consume?metadata=samltoolkit|ISV9.2|primary|z",
            "redirectUris": [
                "https://samltoolkit.azurewebsites.net/SAML/Consume"
            ]
        }
    },
    "servicePrincipal": {
        "id": "912729dd-97ae-4ceb-ade4-07bed3046486",
        "deletedDateTime": null,
        "accountEnabled": true,
        "appId": "3c653ec4-4e4c-4820-8127-49e3889cad99",
        "applicationTemplateId": "229946b9-a9fb-45b8-9531-efa47453ac9e",
        "appDisplayName": "Azure AD SAML Toolkit",
        "alternativeNames": [],
        "appOwnerOrganizationId": "29a4f813-9274-4e1b-858d-0afa98ae66d4",
        "displayName": "Azure AD SAML Toolkit",
        "appRoleAssignmentRequired": true,
        "loginUrl": null,
        "logoutUrl": null,
        "homepage": "https://samltoolkit.azurewebsites.net/SAML/Consume?metadata=samltoolkit|ISV9.2|primary|z",
        "notificationEmailAddresses": [],
        "preferredSingleSignOnMode": null,
        "preferredTokenSigningKeyThumbprint": null,
        "replyUrls": [
            "https://samltoolkit.azurewebsites.net/SAML/Consume"
        ],
        "servicePrincipalNames": [
            "3c653ec4-4e4c-4820-8127-49e3889cad99"
        ],
        "servicePrincipalType": "Application",
        "tags": [
            "WindowsAzureActiveDirectoryIntegratedApp"
        ],
        "tokenEncryptionKeyId": null,
        "samlSingleSignOnSettings": null,
        "verifiedPublisher": {
            "displayName": null,
            "verifiedPublisherId": null,
            "addedDateTime": null
        },
        "addIns": [],
        "appRoles": [
            {
                "allowedMemberTypes": [
                    "User"
                ],
                "displayName": "msiam_access",
                "id": "8b292bda-39b6-4b77-849e-887565235bb0",
                "isEnabled": true,
                "description": "msiam_access",
                "value": null,
                "origin": "Application"
            }
        ],
        "info": {
            "logoUrl": null,
            "marketingUrl": null,
            "privacyStatementUrl": null,
            "supportUrl": null,
            "termsOfServiceUrl": null
        },
        "keyCredentials": [],
        "oauth2PermissionScopes": [
            {
                "adminConsentDescription": "Allow the application to access Azure AD SAML Toolkit on behalf of the signed-in user.",
                "adminConsentDisplayName": "Access Azure AD SAML Toolkit",
                "id": "00e7ef81-4deb-41d7-9ee3-90d4eba1e991",
                "isEnabled": true,
                "type": "User",
                "userConsentDescription": "Allow the application to access Azure AD SAML Toolkit on your behalf.",
                "userConsentDisplayName": "Access Azure AD SAML Toolkit",
                "value": "user_impersonation"
            }
        ],
        "passwordCredentials": []
    }
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationTemplate: instantiate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
