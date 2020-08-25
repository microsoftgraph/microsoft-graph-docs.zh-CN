---
title: 使用 Microsoft Graph Api 配置应用程序代理
description: 使用 Microsoft Graph Api 自动配置应用程序代理，以提供对本地应用程序的远程访问和单一登录。
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cc99857905a0a308f49ddc41bf22da993ca8f1b4
ms.sourcegitcommit: ef47b165f7a140cfc0309a275cb8722dd265660d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2020
ms.locfileid: "46873102"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a>使用 Microsoft Graph API 自动配置应用程序代理

在本文中，您将了解如何为应用程序创建和配置 Azure Active Directory (Azure AD) [应用程序代理](https://aka.ms/whyappproxy) 。 应用程序代理提供了对本地 web 应用程序的安全远程访问和单一登录。 为应用程序配置应用程序代理后，用户可以通过外部 URL、"我的应用程序" 门户或其他内部应用程序门户访问其本地应用程序。

本文假定您已经安装了连接器并完成了应用程序代理的 [先决条件](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin) ，以便连接器可以与 Azure AD 服务进行通信。

请确保你具有相应的权限来调用以下 API。

|资源类型 |方法 |
|---------|---------|
|[applications](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)<br> [onPremisesPublishing](https://docs.microsoft.com/graph/api/resources/onpremisespublishing?view=graph-rest-beta)| [创建应用程序](https://docs.microsoft.com/graph/api/application-post-applications?view=graph-rest-beta&tabs=http) <br> [更新应用程序](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-beta)<br> [向 connectorGroup 添加应用程序](https://docs.microsoft.com/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[连接器](https://docs.microsoft.com/graph/api/resources/connector?view=graph-rest-beta)| [获取连接器](https://docs.microsoft.com/graph/api/connector-get?view=graph-rest-beta)
|[connectorGroup](https://docs.microsoft.com/graph/api/resources/connectorGroup?view=graph-rest-beta)| [Create connectorGroup](https://docs.microsoft.com/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [Add connector to connectorGroup](https://docs.microsoft.com/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[servicePrincipals](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[创建 servicePrincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals?view=graph-rest-beta&tabs=http) <br> [更新 servicePrincipal](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [创建 appRoleAssignments](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

> [!NOTE]
> 本文中所示的请求使用示例值。 你将需要更新这些。 显示的响应对象可能还会缩短可读性。 

## <a name="step-1-create-an-application"></a>步骤1：创建应用程序

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a>登录到 Microsoft Graph Explorer（推荐），Postman 或使用的任何其他 API 客户端

1. 启动 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。
2. 选择 **"使用 Microsoft 登录"** ，并使用 Azure AD 全局管理员或应用程序管理员凭据登录。
3. 成功登录后，将在左窗格中看到用户帐户详细信息。

### <a name="create-an-application"></a>创建应用程序

若要使用 API 为应用程序配置应用程序代理，请创建应用程序，将服务主体添加到应用中，然后更新应用程序的 **onPremisesPublishing** 属性以配置应用程序代理设置。 在创建应用程序时，将应用程序的 **signInAudience** 设置为 "AzureADMyOrg"。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_application"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applications
Content-type: application/json

{
  "displayName": "Contoso IWA App",
  "signInAudience":"AzureADMyOrg"
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#applications/$entity",
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "deletedDateTime": null,
  "addIns": [],
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
  "applicationTemplateId": null,
  "identifierUris": [],
  "createdDateTime": "2020-08-11T21:07:47.5919755Z",
  "description": null,
  "displayName": "Contoso IWA App",
  "isAuthorizationServiceEnabled": false,
  "isDeviceOnlyAuthSupported": null,
  "isFallbackPublicClient": null,
  "groupMembershipClaims": null,
  "notes": null,
  "optionalClaims": null,
  "orgRestrictions": [],
  "publisherDomain": "f128.info",
  "signInAudience": "AzureADandPersonalMicrosoftAccount",
  "tags": [],
  "tokenEncryptionKeyId": null,
  "uniqueName": null,
  "verifiedPublisher": {
      "displayName": null,
      "verifiedPublisherId": null,
      "addedDateTime": null
  },
}
```

### <a name="retrieve-the-application-object-id-and-appid"></a>检索应用程序对象 ID 和 appId
使用上一次调用的响应检索并保存应用程序对象 ID 和应用程序 ID。
```
"application": {
  "id": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b"
}
```
### <a name="create-a-serviceprincipal-for-the-application-and-add-required-tags"></a>为应用程序创建一个 servicePrincipal 并添加所需的标记
使用 **appId** 为应用程序创建服务主体。 然后添加为应用配置应用程序代理所需的标记。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "create_servicePrincipal"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/serviceprincipals
Content-type: appplication/json

{
  "appId":"d7fbfe28-c60e-46d2-8335-841923950d3b",
  "tags": [
    "WindowsAzureActiveDirectoryIntegratedApp",
    "WindowsAzureActiveDirectoryOnPremApp"
  ]
}
```

#### <a name="response"></a>响应
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application",
  "isCollection": true
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals/$entity",
  "id": "a8cac399-cde5-4516-a674-819503c61313",
  "deletedDateTime": null,
  "accountEnabled": true,
  "alternativeNames": [],
  "createdDateTime": null,
  "deviceManagementAppType": null,
  "appDescription": null,
  "appDisplayName": "Contoso IWA App",
  "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
  "applicationTemplateId": null,
  "appOwnerOrganizationId": "7918d4b5-0442-4a97-be2d-36f9f9962ece",
  "appRoleAssignmentRequired": false,
  "description": null,
  "displayName": "vtestapi2",
  "errorUrl": null,
  "homepage": null,
  "isAuthorizationServiceEnabled": false,
  "loginUrl": null,
  "logoutUrl": null,
  "notes": null,
  "notificationEmailAddresses": [],
  "preferredSingleSignOnMode": null,
  "preferredTokenSigningKeyEndDateTime": null,
  "preferredTokenSigningKeyThumbprint": null,
  "publisherName": "f/128 Photography",
  "replyUrls": [],
  "samlMetadataUrl": null,
  "samlSingleSignOnSettings": null,
  "servicePrincipalNames": [
      "b92b92d4-3874-46a5-b715-a00ea01cff93"
  ],
  "servicePrincipalType": "Application",
}
```

## <a name="step-2-configure-application-proxy-properties"></a>步骤2：配置应用程序代理属性

### <a name="set-the-onpremisespublishing-configuration"></a>设置 onPremisesPublishing 配置

使用上一步中的 application 对象 ID 为应用程序配置应用程序代理，并将 **onPremisesPublishing** 属性更新为所需的配置。 在此示例中，您使用的是内部 URL 的应用程序： `https://contosoiwaapp.com` 并使用外部 url 的默认域： `https://contosoiwaapp-contoso.msappproxy.net` 。 

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
    "onPremisesPublishing": {
        "externalAuthenticationType": "aadPreAuthentication",
        "internalUrl": "https://contosoiwaapp.com",
        "externalUrl": "https://contosoiwaapp-contoso.msappproxy.net"
    }
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="complete-the-configuration-of-the-application"></a>完成应用程序的配置
将应用程序的 " **redirectUri**"、" **identifierUri**" 和 " **HomepageUrl** " 属性更新为 **onPremisesPublishing** 属性中配置的外部 UR。 然后，将 [implicitGrantSettings](https://docs.microsoft.com/graph/api/resources/implicitgrantsettings?view=graph-rest-1.0) 更新为 `true` 针对 **enabledTokenIssuance** 和 `false` **enabledAccessTokenIssuance**。

#### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
  "identifierUris": ["https://contosoiwaapp-contoso.msappproxy.net"],
  "web": {
    "redirectUris": ["https://contosoiwaapp-contoso.msappproxy.net"],
    "homePageUrl": "https://contosoiwaapp-contoso.msappproxy.net",
    "implicitGrantSettings": {
      "enableIdTokenIssuance": true,
      "enableAccessTokenIssuance": false
    }
  }
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-3-assign-the-connector-group-to-the-application"></a>步骤3：将连接器组分配给应用程序

### <a name="get-connectors"></a>获取连接器

列出连接器并使用响应来检索和保存连接器对象 ID。 连接器对象 ID 将用于将连接器分配给连接器组。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectors",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#connectors",
    "value": [
        {
            "id": "d2b1e8e8-8511-49d6-a4ba-323cb083fbb0",
            "machineName": "connectorA.redmond.contoso.com"",
            "externalIp": "131.137.147.164",
            "status": "active"
        },
        {
            "id": "f2cab422-a1c8-4d70-a47e-2cb297a2e051",
            "machineName": "connectorB.contoso.com"",
            "externalIp": "68.0.191.210",
            "status": "active"
        },
        {
            "id": "8555cc3c-5c8b-48a8-a8b2-5e97c32ef907",
            "machineName": "connectorC.contoso.com",
            "externalIp": "40.78.66.161",
            "status": "active"
        }
    ]
}
```

### <a name="create-a-connectorgroup"></a>创建 connectorGroup
在此示例中，创建了一个用于应用程序的名为 "IWA Demo Connector Group" 的新 connectorGroup。 如果您的连接器已分配给相应的 connectorGroup，也可以跳过此步骤。 检索并保存要在下一步中使用的 connectorGroup 对象 ID。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups

Content-type: application/json
{
   "name": "IWA Demo Connector Group"
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 201
Content-type: connectorGroup/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#connectorGroups/$entity",
    "id": "3e6f4c35-a04b-4d03-b98a-66fff89b72e6",
    "name": "IWA Demo Connector Group",
    "connectorGroupType": "applicationProxy",
    "isDefault": false
}
```

### <a name="assign-a-connector-to-the-connectorgroup"></a>将连接器分配给 connectorGroup

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/8555cc3c-5c8b-48a8-a8b2-5e97c32ef907/memberOf/$ref

Content-type: application/json
{
  "@odata.id":"https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

### <a name="assign-the-application-to-the-connectorgroup"></a>将应用程序分配给 connectorGroup

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "connectorGroup"
}-->

```msgraph-interactive
PUT https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83/connectorGroup/$ref
Content-type: application/json

{
"@odata.id":"https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/3e6f4c35-a04b-4d03-b98a-66fff89b72e6"
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a>步骤4：配置单一登录
此应用程序使用集成的 Windows 身份验证 (IWA) 。 若要配置 IWA，请在 [singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta) 资源类型中设置单一登录属性。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "update_application"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/bf21f7e9-9d25-4da2-82ab-7fdd85049f83
Content-type: appplication/json

{
   "onPremisesPublishing": {
      "singleSignOnSettings": {
         "kerberosSignOnSettings": {
            "kerberosServicePrincipalName": "HTTP/iwademo.contoso.com",
        "kerberosSignOnMappingAttributeType": "userPrincipalName"
         },
         "singleSignOnMode": "onPremisesKerberos"
      }
   }
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-5-assign-users"></a>第 5 步：分配用户
### <a name="retrieve-approle-for-the-applicaiton"></a>检索应用程序的 appRole

#### <a name="request"></a>请求


<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/a8cac399-cde5-4516-a674-819503c61313/appRoles
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('a8cac399-cde5-4516-a674-819503c61313')/appRoles",
    "value": [
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        },
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "msiam_access",
            "displayName": "msiam_access",
            "id": "b9632174-c057-4f7e-951b-be3adc52bfe6",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        }
    ]
}
```

使用上一次调用中的响应检索并保存 appRole ID 以用于下一步。
```
      {
            "description": "User",
            "displayName": "User",
            "id": "18d14569-c3bd-439b-9a66-3a2aee01d14f"
        }
```

### <a name="assign-users-and-groups-to-the-application"></a>向应用程序分配用户和组

使用以下属性将用户分配给应用程序。

| 属性  | 说明 |ID  |
|---------|---------|---------|
| principalId | 将分配给应用程序的用户的用户 ID | 2fe96d23-5dc6-4f35-8222-0426a8c115c8 |
| principalType | 用户类型 | 用户 |
| appRoleId |  应用程序的默认应用程序角色的应用程序角色 ID | 18d14569-c3bd-439b-9a66-3a2aee01d14f |
| resourceId | 应用程序的 servicePrincipal ID | a8cac399-cde5-4516-a674-819503c61313 |

#### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoleAssignments

Content-type: appRoleAssignments/json

{
  "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
  "principalType": "User",
  "appRoleId":"18d14569-c3bd-439b-9a66-3a2aee01d14f",
  "resourceId":"a8cac399-cde5-4516-a674-819503c61313"
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appRoleAssignments/$entity",
    "id": "I23pL8ZdNU-CIgQmqMEVyLJ0E6fx0ixEo92az8MnhtU",
    "creationTimestamp": "2020-06-09T00:06:07.5129268Z",
    "appRoleId": "18d14569-c3bd-439b-9a66-3a2aee01d14f",
    "principalDisplayName": "Jean Green",
    "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
    "principalType": "User",
    "resourceDisplayName": "Contoso IWA App",
    "resourceId": "a8cac399-cde5-4516-a674-819503c61313"
}
```

有关详细信息，请参阅 [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta) 资源类型。


## <a name="additional-steps"></a>其他步骤
- [使用 PowerShell 示例为应用程序代理自动执行配置](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [使用 Microsoft Graph API 自动化基于 SAML 的 SSO 应用配置](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)
