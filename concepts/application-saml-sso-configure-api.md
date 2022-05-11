---
title: 使用 Microsoft Graph API 配置基于 SAML 的单一登录
description: 了解如何通过使用 Microsoft Graph API 来自动配置基于 SAML 的单一登录来节省时间。
author: kenwith
ms.localizationpriority: high
ms.custom: scenarios:getting-started
ms.prod: applications
ms.openlocfilehash: 06fb882695affc40898d7c9391f655e0bdccfff7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65314821"
---
# <a name="configure-saml-based-single-sign-on-for-your-application-using-the-microsoft-graph-api"></a>使用 Microsoft Graph API 为应用程序配置基于 SAML 的单一登录

本文介绍了如何使用 Microsoft Graph API 为 Azure Active Directory （Azure AD） 中的应用程序创建和配置基于 SAML 的单一登录 （SSO）。 应用程序配置包括基本 SAML URL、声明映射策略以及使用证书添加自定义签名密钥。 创建应用程序后，可以为其分配管理员用户。 然后，可以使用 URL 获取 Azure AD SAML 元数据，以对应用程序进行其他配置。 

本文使用 AWS Azure AD 应用程序模板作为示例，但可以针对 Azure AD 库中的任何基于 SAML 的应用使用本文中的步骤。

## <a name="prerequisites"></a>先决条件

本教程的前提是使用 Microsoft Graph Explorer，但是可以使用 Postman，也可以创建自己的客户端应用程序来调用 Microsoft Graph。 如果要在本教程中调用 Microsoft Graph API，需要使用具有全局管理员角色和适当权限的帐户。 对于本教程，需要`Application.ReadWrite.All`、`AppRoleAssignment.ReadWrite.All`、`Policy.Read.All`、`Policy.ReadWrite.ApplicationConfiguration` 和 `User.ReadWrite.All` 委派权限。 完成以下步骤以在 Microsoft Graph 浏览器中设置权限：

1. 转到 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。
2. 选择“**使用 Microsoft 登录**”，然后使用 Azure AD 全局管理员账户登录。 成功登录后，可在左侧窗格中看到用户帐户详细信息。
3. 选择用户帐户详细信息右侧的设置图标，然后选择“**权限**”。

    ![选择 Microsoft Graph 权限](./images/application-saml-sso-configure-api/set-permissions.png)
        
4. 在权限列表中，滚动到并展开“**AppRoleAssignment (1)**”，然后选择“**AppRoleAssignment.ReadWrite.All**”权限。 继续向下滚动并展开“**应用程序 (2)**”，然后选择“**Application.ReadWrite.All**”权限。 继续滚动到并选择“**策略 (13)**”，然后选择“**Policy.Read.All**”和“**Policy.ReadWrite.ApplicationConfiguration**”权限。 最后，滚动到并展开“**用户 (8)**”，然后选择“**User.ReadWrite.All**”。

    ![滚动并选择 approleasignment、应用程序和策略权限](./images/application-saml-sso-configure-api/select-permissions.png)

5. 选择“**同意**”，然后选择“**接受**”，以接受同意权限。 你不需要代表组织同意这些权限。

    ![接受同意权限](./images/application-saml-sso-configure-api/accept-permissions.png)

## <a name="step-1-create-the-application"></a>第 1 步：创建应用程序

Azure AD 中存在一个库，其中包含数千个预集成的应用程序，可以将其用作应用程序的模板。 应用程序模板描述了该应用程序的元数据。 使用此模板，可以在租户中创建应用程序和服务主体的实例以进行管理。 

如果要从库中创建应用程序，首先获取应用程序模板的标识符，然后使用该标识符创建应用程序。

### <a name="retrieve-the-gallery-application-template-identifier"></a>检索库应用程序模板标识符

 在本教程中，将检索 `AWS Single Sign-on` 应用程序模板的标识符。 记录 **id** 属性值，以供稍后在本教程中使用。

#### <a name="request"></a>请求

```http
GET https://graph.microsoft.com/v1.0/applicationTemplates?$filter=displayName eq 'AWS Single Sign-on'
```

#### <a name="response"></a>响应

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applicationTemplates",
  "value": [
    {
      "id": "21ed01d2-ec13-4e9e-86c1-cd546719ebc4",
      "displayName": "AWS Single Sign-on",
      "homePageUrl": "https://aws.amazon.com/",
      "supportedSingleSignOnModes": [
        "saml",
        "external"
      ],
      "supportedProvisioningTypes": [
        "sync"
      ],
      "logoUrl": "https://az495088.vo.msecnd.net/app-logo/awssinglesignon_215.png",
      "categories": [
        "developerServices",
        "itInfrastructure",
        "security",
        "New"
      ],
      "publisher": "Amazon Web Services, Inc.",
      "description": "Federate once to AWS SSO & use it to manage access centrally to multiple AWS accounts. Provision users via SCIM & get Azure AD single sign-in access to the AWS Console, CLI, & AWS SSO integrated apps."
    }
  ]
}
```

### <a name="create-the-application"></a>创建应用程序

使用为应用模板记录的 **id** 值，在租户中为应用和服务主题创建实例。 记录应用程序的 **id** 属性值和服务主体的 **id** 属性值，以在本教程中稍后使用。

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/applicationTemplates/21ed01d2-ec13-4e9e-86c1-cd546719ebc4/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
}
```

> [!NOTE]
> 留出一些时间将应用程序配置到 Azure AD 租户中。 这不是即时的。 一种策略是每 5-10秒 对应用程序或服务主体对象执行 GET 查询，直到查询成功。

#### <a name="response"></a>响应

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.applicationServicePrincipal",
  "application": {
    "id": "a9be408a-6c31-4141-8cea-52fcd4a61be8",
    "appId": "17cad0e7-cd2b-4e51-a75d-ba810f3e4045",
    "applicationTemplateId": "21ed01d2-ec13-4e9e-86c1-cd546719ebc4",
    "createdDateTime": "2021-05-10T20:12:03Z",
    "deletedDateTime": null,
    "displayName": "AWS Contoso",
    "groupMembershipClaims": null,
    "identifierUris": [],
    "isFallbackPublicClient": false,
    "signInAudience": "AzureADMyOrg",
    "tags": [],
    "tokenEncryptionKeyId": null,
    "defaultRedirectUri": null,
    "optionalClaims": null,
    "verifiedPublisher": {
      "displayName": null,
      "verifiedPublisherId": null,
      "addedDateTime": null
    },
    "addIns": [],
    "api": {
      "acceptMappedClaims": null,
      "knownClientApplications": [],
      "requestedAccessTokenVersion": null,
      "oauth2PermissionScopes": [
        {
          "adminConsentDescription": "Allow the application to access AWS Contoso on behalf of the signed-in user.",
          "adminConsentDisplayName": "Access AWS Contoso",
          "id": "6f891cd3-c132-4822-930b-f343b4515d19",
          "isEnabled": true,
          "type": "User",
          "userConsentDescription": "Allow the application to access AWS Contoso on your behalf.",
          "userConsentDisplayName": "Access AWS Contoso",
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
        "displayName": "User",
        "id": "8774f594-1d59-4279-b9d9-59ef09a23530",
        "isEnabled": true,
        "description": "User",
        "value": null,
        "origin": "Application"
      },
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "msiam_access",
        "id": "e7f1a7f3-9eda-48e0-9963-bd67bf531afd",
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
    "web": {
      "homePageUrl": "https://*.signin.aws.amazon.com/platform/saml/acs/*?metadata=awssinglesignon|ISV9.1|primary|z",
      "redirectUris": []
    }
  },
  "servicePrincipal": {
    "id": "a750f6cf-2319-464a-bcc3-456926736a91",
    "deletedDateTime": null,
    "accountEnabled": true,
    "appId": "17cad0e7-cd2b-4e51-a75d-ba810f3e4045",
    "applicationTemplateId": "21ed01d2-ec13-4e9e-86c1-cd546719ebc4",
    "appDisplayName": "AWS Contoso",
    "alternativeNames": [],
    "appOwnerOrganizationId": "8500cad3-193d-48a6-8d00-c129b114dc10",
    "displayName": "AWS Contoso",
    "appRoleAssignmentRequired": true,
    "loginUrl": null,
    "logoutUrl": null,
    "homepage": "https://*.signin.aws.amazon.com/platform/saml/acs/*?metadata=awssinglesignon|ISV9.1|primary|z",
    "notificationEmailAddresses": [],
    "preferredSingleSignOnMode": null,
    "preferredTokenSigningKeyThumbprint": null,
    "replyUrls": [],
    "servicePrincipalNames": [
      "17cad0e7-cd2b-4e51-a75d-ba810f3e4045"
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
        "displayName": "User",
        "id": "8774f594-1d59-4279-b9d9-59ef09a23530",
        "isEnabled": true,
        "description": "User",
        "value": null,
        "origin": "Application"
      },
      {
        "allowedMemberTypes": [
          "User"
        ],
        "displayName": "msiam_access",
        "id": "e7f1a7f3-9eda-48e0-9963-bd67bf531afd",
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
        "adminConsentDescription": "Allow the application to access AWS Contoso on behalf of the signed-in user.",
        "adminConsentDisplayName": "Access AWS Contoso",
        "id": "6f891cd3-c132-4822-930b-f343b4515d19",
        "isEnabled": true,
        "type": "User",
        "userConsentDescription": "Allow the application to access AWS Contoso on your behalf.",
        "userConsentDisplayName": "Access AWS Contoso",
        "value": "user_impersonation"
      }
    ],
    "passwordCredentials": []
  }
}
```

## <a name="step-2-configure-single-sign-on"></a>第 2 步：配置单一登录

在本教程中，`saml`设置为服务主体中的单一登录模式。 使用之前记录的服务主体 **id**。

#### <a name="request"></a>请求

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91
Content-type: application/json

{
  "preferredSingleSignOnMode": "saml"
}
```

#### <a name="response"></a>响应

```http
HTTP/1.1 204
```

### <a name="set-basic-saml-urls"></a>设置基本 SAML URL

使用之前记录的应用程序 **id**，设置标识符 URI，并在应用程序对象中重定向 AWS 的 URI。

#### <a name="request"></a>请求

```http
PATCH https://graph.microsoft.com/v1.0/applications/a9be408a-6c31-4141-8cea-52fcd4a61be8
Content-type: application/json

{
  "web": {
    "redirectUris": [
      "https://signin.aws.amazon.com/saml"
    ] 
  },
  "identifierUris": [
    "https://signin.aws.amazon.com/saml"
  ]    
}
```

#### <a name="response"></a>响应

```http
HTTP/1.1 204
```

### <a name="add-app-roles-optional"></a>添加应用程序角色（可选）

如果应用程序需要令牌中的角色信息，请在应用程序对象中添加角色的定义。 

> [!NOTE] 
> 添加应用程序角色时，请勿修改默认应用程序角色 `msiam_access`。 

使用之前记录的服务主体 **id**。

#### <a name="request"></a>请求

```http
PATCH https://graph.microsoft.com/v1.0/serviceprincipals/a750f6cf-2319-464a-bcc3-456926736a91
Content-type: application/json

{
  "appRoles": [
    {
      "allowedMemberTypes": [
        "User"
      ],
      "displayName": "User",
      "id": "8774f594-1d59-4279-b9d9-59ef09a23530",
      "isEnabled": true,
      "description": "User",
      "value": null,
      "origin": "Application"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "displayName": "msiam_access",
      "id": "e7f1a7f3-9eda-48e0-9963-bd67bf531afd",
      "isEnabled": true,
      "description": "msiam_access",
      "value": null,
      "origin": "Application"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "Admin,WAAD",
      "displayName": "Admin,WAAD",
      "id": "3a84e31e-bffa-470f-b9e6-754a61e4dc63",
      "isEnabled": true,
      "value": "arn:aws:iam::212743507312:role/accountname-aws-admin,arn:aws:iam::212743507312:saml-provider/WAAD"
    },
    {
      "allowedMemberTypes": [
        "User"
      ],
      "description": "Finance,WAAD",
      "displayName": "Finance,WAAD",
      "id": "7a960000-ded3-455b-8c04-4f2ace00319b",
      "isEnabled": true,
      "value": "arn:aws:iam::212743507312:role/accountname-aws-finance,arn:aws:iam::212743507312:saml-provider/WAAD"
    }
  ]
}
```

#### <a name="response"></a>响应

```http
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a>第 3 步：配置声明映射

### <a name="create-a-claims-mapping-policy"></a>创建声明映射策略

除了基本声明之外，还为 Azure AD 配置以下声明以在 SAML 令牌中发出：

| 声明名称 | 源  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | assignedroles| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | userprincipalname |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | "900" |
| roles | assignedroles |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | userprincipalname |

> [!NOTE]
> 声明映射策略中的某些项区分大小写（例如“Version”）。 如果收到错误消息，例如“属性的值无效”，则可能是区分大小写的问题。

创建声明映射策略并创建 **id**，以随后在本教程中使用。

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies
Content-type: application/json

{
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Value\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
    ],
    "displayName": "AWS Claims Policy",
    "isOrganizationDefault": false
}
```

#### <a name="response"></a>响应

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/claimsMappingPolicies/$entity",
    "id": "4bce7ba7-466d-4239-94b8-cf4f21428ca7",
    "deletedDateTime": null,
    "definition": [
        "{\"ClaimsMappingPolicy\":{\"Version\":1,\"IncludeBasicClaimSet\":\"true\", \"ClaimsSchema\": [{\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"}, {\"Value\":\"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"}, {\"Source\":\"user\",\"ID\":\"assignedroles\",\"SamlClaimType\": \"appRoles\"}, {\"Source\":\"user\",\"ID\":\"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/nameidentifier\"}]}}"
    ],
    "displayName": "AWS Claims Policy",
    "isOrganizationDefault": false
}
```

### <a name="assign-a-claims-mapping-policy-to-a-service-principal"></a>向服务主体分配声明映射策略

使用之前记录的服务主体 **id** 为其分配映射策略。 将 **id** 属性值用于请求正文中的声明映射策略。

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91/claimsMappingPolicies/$ref
Content-type: application/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/a4b35718-fd5e-4ca8-8248-a3c9934b1b78"
}
```

#### <a name="response"></a>响应

```http
HTTP/1.1 204
```

## <a name="step-4-configure-a-signing-certificate"></a>第 4 步：配置签名证书

你需要一个自签名证书，Azure AD 可以使用该证书来签署 SAML 响应。 可以使用自己的证书，也可以使用以下示例。 

### <a name="create-a-signing-certificate"></a>创建签名证书

使用所创建的服务主体 **id**，创建新的证书并将其添加到服务主体。

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91/addTokenSigningCertificate
Content-type: application/json

{
    "displayName":"CN=AWSContoso",
    "endDateTime":"2024-01-25T00:00:00Z"
}
```

#### <a name="response"></a>响应

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.selfSignedCertificate",
  "customKeyIdentifier": "p9PEYmuKhP2oaMzGfSdNQC/9ChA=",
  "displayName": "CN=AWSContoso",
  "endDateTime": "2024-01-25T00:00:00Z",
  "key": "MIICqjCCAZKgAwIBAgIId....4rnrk43wp75yqjRbOhAZ1ExAxVqW+o2JslhjUeltUMNQW+ynOfs9oHu1ZdnGmxrE=",
  "keyId": "70883316-50be-4016-ba80-19d9fbad873d",
  "startDateTime": "2021-05-10T20:35:37.5754318Z",
  "thumbprint": "A7D3C4626B8A84FDA868CCC67D274D402FFD0A10",
  "type": "AsymmetricX509Cert",
  "usage": "Verify"
}
```

### <a name="activate-the-custom-signing-key"></a>激活自定义签名密钥

需要将服务主体的 **preferredTokenSigningKeyThumbprint** 属性设置为想要Azure AD 用于签署 SAML 响应的证书指纹。 

#### <a name="request"></a>请求

```http
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91
Content-type: application/json

{
  "preferredTokenSigningKeyThumbprint": "A7D3C4626B8A84FDA868CCC67D274D402FFD0A10"
}
```

#### <a name="response"></a>响应

```http
HTTP/1.1 204
```

## <a name="step-5-assign-users"></a>第 5 步：分配用户

### <a name="create-a-user-account"></a>创建用户账户

对于本教程，将创建一个添加到应用程序中的用户帐户。 在请求正文中，将 contoso.com 更改为租户的域名。 可在 Azure Active Directory 概述页面上找到租户信息。 记录要在本教程后面要使用的用户 **id**。

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/users
Content-type: application/json

{
  "accountEnabled":true,
  "displayName":"MyTestUser1",
  "mailNickname":"MyTestUser1",
  "userPrincipalName":"MyTestUser1@contoso.com",
  "passwordProfile": {
    "forceChangePasswordNextSignIn":true,
    "password":"Contoso1234"
  }
}
```

#### <a name="response"></a>响应

```http
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users/$entity",
  "id": "040f9599-7c0f-4f94-aa75-8394c4c6ea9b",
  "businessPhones": [],
  "displayName": "MyTestUser1",
  "userPrincipalName": "MyTestUser1@contoso.com"
}
```

### <a name="assign-a-user-to-the-application"></a>向应用程序分配用户

将创建的用户分配给服务主体，然后分配 `Admin,WAAD` 应用程序角色。 

在请求正文中，提供这些值：

- **principalId** - 所创建的用户账户的 **id**。
- **appRoleId** - 新增 `Admin,WAAD` 应用程序角色的 **id**。
- **resourceId** - 服务主体的 **id**。

#### <a name="request"></a>请求

```http
POST https://graph.microsoft.com/v1.0/servicePrincipals/a750f6cf-2319-464a-bcc3-456926736a91/appRoleAssignments
Content-type: application/json

{
  "principalId": "040f9599-7c0f-4f94-aa75-8394c4c6ea9b",
  "principalType": "User",
  "appRoleId":"3a84e31e-bffa-470f-b9e6-754a61e4dc63",
  "resourceId":"a750f6cf-2319-464a-bcc3-456926736a91"
}
```

#### <a name="response"></a>响应

```http
HTTP/1.1 201 
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals('a750f6cf-2319-464a-bcc3-456926736a91')/appRoleAssignments/$entity",
  "id": "mZUPBA98lE-qdYOUxMbqm2qY3odGRGdFtpYJkAfUC0Q",
  "deletedDateTime": null,
  "appRoleId": "3a84e31e-bffa-470f-b9e6-754a61e4dc63",
  "createdDateTime": "2021-05-10T21:04:11.0480851Z",
  "principalDisplayName": "MyTestUser1",
  "principalId": "040f9599-7c0f-4f94-aa75-8394c4c6ea9b",
  "principalType": "User",
  "resourceDisplayName": "AWS Contoso",
  "resourceId": "a750f6cf-2319-464a-bcc3-456926736a91"
}
```

## <a name="step-6-get-azure-ad-saml-metadata"></a>第 6 步：获取 Azure AD SAML 元数据

使用以下 URL 获取特定配置的应用程序的 Azure AD SAML 元数据。 元数据包含诸如签名证书、Azure AD entityID和 Azure AD SingleSignOnService 等信息。

`https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`

下面显示了可能在应用程序中看到的示例：

```
<EntityDescriptor xmlns="urn:oasis:names:tc:SAML:2.0:metadata" ID="_05fbbf53-e892-43c9-9300-1f6738ace02c" entityID="https://sts.windows.net/2f82f566-5953-43f4-9251-79c6009bdf24/">
<Signature xmlns="http://www.w3.org/2000/09/xmldsig#">

...

<SingleLogoutService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
<SingleSignOnService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
<SingleSignOnService Binding="urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST" Location="https://login.microsoftonline.com/2f82f566-5953-43f4-9251-79c6009bdf24/saml2"/>
</IDPSSODescriptor>
</EntityDescriptor>
```

## <a name="step-7-clean-up-resources"></a>第 7 步：清理资源

在此步骤中，将删除创建的资源。


### <a name="delete-the-application"></a>删除应用程序

删除创建的应用程序。

#### <a name="request"></a>请求

```http
DELETE https://graph.microsoft.com/v1.0/applications/a9be408a-6c31-4141-8cea-52fcd4a61be8
```

#### <a name="response"></a>响应

```http
No Content - 204
```

### <a name="delete-the-user-account"></a>删除用户账户

删除 MyTestUser1 用户帐户。

#### <a name="request"></a>请求

```http
DELETE https://graph.microsoft.com/v1.0/users/040f9599-7c0f-4f94-aa75-8394c4c6ea9b
```

#### <a name="response"></a>响应

```http
No Content - 204
```

### <a name="delete-the-claims-mapping-policy"></a>删除声明映射策略

删除声明映射策略。

#### <a name="request"></a>请求

```http
DELETE https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/a4b35718-fd5e-4ca8-8248-a3c9934b1b78
```

#### <a name="response"></a>响应

```http
No Content - 204
```

## <a name="see-also"></a>另请参阅

- 对于 AWS，可以[启用用户配置](/azure/active-directory/app-provisioning/application-provisioning-configuration-api)以从该 AWS 账户获取所有角色。 有关详细信息，请参阅[配置 SAML 令牌中颁发的角色声明](/azure/active-directory/develop/active-directory-enterprise-app-role-management)。
- [自定义在租户具体应用的令牌中颁发的声明](/azure/active-directory/develop/active-directory-claims-mapping)。
- 可以使用 applicationTemplate API 来实例化非库应用程序。[非库应用](/azure/active-directory/manage-apps/view-applications-portal)。使用 applicationTemplateId`8adf8e6e-67b2-4cf2-a259-e3dc5476c621`。
- [applicationTemplate](/graph/api/resources/applicationtemplate)
- [appRoleAssignment](/graph/api/resources/approleassignment)
- [servicePrincipal](/graph/api/resources/serviceprincipal)
- [application](/graph/api/resources/application)
- [claimsMappingPolicy](/graph/api/resources/claimsmappingpolicy)
- [keyCredential](/graph/api/resources/keycredential)
- [addTokenSigningCertificate](/graph/api/serviceprincipal-addtokensigningcertificate)
