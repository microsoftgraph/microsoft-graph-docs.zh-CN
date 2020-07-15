---
title: 使用 Microsoft Graph Api 配置应用程序代理
description: 使用 Microsoft Graph Api 自动配置应用程序代理，以提供对本地应用程序的远程访问和单一登录。
author: davidmu1
ms.topic: conceptual
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 065e7cdc84a353c4636fc4e7d13c32d22c7bce70
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142340"
---
# <a name="automate-the-configuration-of-application-proxy-using-the-microsoft-graph-api"></a>使用 Microsoft Graph API 自动配置应用程序代理

在本文中，您将了解如何为应用程序创建和配置 Azure Active Directory （Azure AD）[应用程序代理](https://aka.ms/whyappproxy)。 应用程序代理提供了对本地 web 应用程序的安全远程访问和单一登录。 为应用程序配置应用程序代理后，用户可以通过外部 URL、"我的应用程序" 门户或其他内部应用程序门户访问其本地应用程序。

本文假定您已经安装了连接器并完成了应用程序代理的[先决条件](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application#before-you-begin)，以便连接器可以与 Azure AD 服务进行通信。

请确保您具有调用以下 Api 的相应权限。

|资源类型 |方法 |
|---------|---------|
| [applicationTemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta)| [实例化 applicationTemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta) |
|[来说](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)<br> [onPremisesPublishing](https://docs.microsoft.com/graph/api/resources/onpremisespublishing?view=graph-rest-beta)|[更新应用程序](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-beta)<br> [向 connectorGroup 添加应用程序](https://docs.microsoft.com/graph/api/connectorgroup-post-applications?view=graph-rest-beta)|
|[连接器](https://docs.microsoft.com/graph/api/resources/connector?view=graph-rest-beta)| [获取连接器](https://docs.microsoft.com/graph/api/connector-get?view=graph-rest-beta)
|[connectorGroup](https://docs.microsoft.com/graph/api/resources/connectorGroup?view=graph-rest-beta)| [创建 connectorGroup](https://docs.microsoft.com/graph/api/resources/connectorgroup?view=graph-rest-beta) <br> [将连接器添加到 connectorGroup](https://docs.microsoft.com/graph/api/connector-post-memberof?view=graph-rest-beta) <br> |
|[servicePrincipals](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[更新 servicePrincipal](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [创建 appRoleAssignments](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-beta)|

>[!NOTE]
> 本文中所示的请求使用示例值。 你将需要更新这些。 为了提高可读性，还可能缩短了显示的响应对象。 所有属性都将通过实际调用返回。

## <a name="step-1-create-a-custom-application"></a>步骤1：创建自定义应用程序

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a>登录到 Microsoft Graph 浏览器（推荐）、Postman 或任何其他使用的 API 客户端

1. 启动[Microsoft Graph 资源管理器](https://developer.microsoft.com/graph/graph-explorer)。
2. 选择 **"使用 Microsoft 登录"** ，并使用 Azure AD 全局管理员或应用程序管理员凭据登录。
3. 登录成功后，将在左窗格中看到用户帐户详细信息。

### <a name="create-a-custom-application"></a>创建自定义应用程序

若要使用 API 为应用程序配置应用程序代理，您必须首先创建自定义应用程序，然后更新应用程序的**onPremisesPublishing**属性，以配置应用程序代理设置。
使用[实例化 applicationTemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta)在租户中创建自定义应用程序和服务主体的实例，以供管理。 自定义应用程序的模板 ID 为： `8adf8e6e-67b2-4cf2-a259-e3dc5476c621` 。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_applicationTemplate"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applicationTemplates/8adf8e6e-67b2-4cf2-a259-e3dc5476c621/instantiate
Content-type: application/json

{
  "displayName": "Contoso IWA App"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-applicationtemplate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-applicationtemplate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-applicationtemplate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#microsoft.graph.applicationServicePrincipal",
    "application": {
        "objectId": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83",
        "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
        "applicationTemplateId": "8adf8e6e-67b2-4cf2-a259-e3dc5476c621",
        "displayName": "Contoso IWA App",
        "homepage": "https://account.activedirectory.windowsazure.com:444/applications/default.aspx?metadata=customappsso|ISV9.1|primary|z",
        "identifierUris": [],
        "publicClient": null,
        "replyUrls": [],
        "logoutUrl": null,
        "samlMetadataUrl": null,
        "errorUrl": null,
        "groupMembershipClaims": null,
        "availableToOtherTenants": false
    },
    "servicePrincipal": {
        "objectId": "b00c693f-9658-4c06-bd1b-c402c4653dea",
        "deletionTimestamp": null,
        "accountEnabled": true,
        "appId": "d7fbfe28-c60e-46d2-8335-841923950d3b",
        "appDisplayName": "Contoso API",
        "applicationTemplateId": "8adf8e6e-67b2-4cf2-a259-e3dc5476c621",
        "appRoleAssignmentRequired": true,
        "displayName": "Contoso API",
        "errorUrl": null,
        "logoutUrl": null,
        "homepage": "https://account.activedirectory.windowsazure.com:444/applications/default.aspx?metadata=customappsso|ISV9.1|primary|z",
        "samlMetadataUrl": null,
        "microsoftFirstParty": null,
        "publisherName": "f/128 Photography",
        "preferredTokenSigningKeyThumbprint": null,
        "replyUrls": [],
        "servicePrincipalNames": [
            "d7fbfe28-c60e-46d2-8335-841923950d3b"
        ],
        "tags": [
            "WindowsAzureActiveDirectoryIntegratedApp",
            "WindowsAzureActiveDirectoryCustomSingleSignOnApplication"
        ],
        "notificationEmailAddresses": [],
        "keyCredentials": [],
        "passwordCredentials": []
    }
}
```


### <a name="retrieve-app-object-id-and-service-principal-object-id"></a>检索应用程序对象 ID 和服务主体对象 ID
使用上一次调用的响应检索并保存 application 对象 ID 和服务主体对象 ID。
```
"application": {
    "objectId": "bf21f7e9-9d25-4da2-82ab-7fdd85049f83"
    }
"servicePrincipal": {
    "objectId": "b00c693f-9658-4c06-bd1b-c402c4653dea"
    }
```

## <a name="step-2-configure-application-proxy-properties"></a>步骤2：配置应用程序代理属性

### <a name="set-the-onpremisespublishing-configuration"></a>设置 onPremisesPublishing 配置

使用上一步中的 applicationId 为应用程序配置应用程序代理，并将**onPremisesPublishing**属性更新为所需的配置。 在此示例中，您使用的是内部 url 的应用程序： `https://contosoiwaapp.com` 并使用外部 url 的默认域： `https://contosoiwaapp-contoso.msappproxy.net` 。 

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```
### <a name="set-the-redirecturi-identifieruri-and-homepageurl-properties"></a>设置 redirectUri、identifierUri 和 homepageUrl 属性
将应用程序的 " **redirectUri**"、" **identifierUri**" 和 " **homepageUrl** " propertes 更新为外部 URL。

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
      "homePageUrl": "https://contosoiwaapp-contoso.msappproxy.net"
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


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connector"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors

```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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


# <a name="http"></a>[HTTP](#tab/http)
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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No content
```

## <a name="step-4-configure-single-sign-on"></a>步骤4：配置单一登录
此应用程序使用集成的 Windows 身份验证（IWA）。 若要配置 IWA，请在[singleSignOnSettings](https://docs.microsoft.com/graph/api/resources/onpremisespublishingsinglesignon?view=graph-rest-beta)资源类型中设置单一登录属性。


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

## <a name="step-5-assign-users"></a>步骤5：分配用户
### <a name="retrieve-approle-for-the-applicaiton"></a>检索应用程序的 appRole

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoles
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/serviceprincipals-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/serviceprincipals-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/serviceprincipals-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 200
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#servicePrincipals('b00c693f-9658-4c06-bd1b-c402c4653dea')/appRoles",
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

### <a name="assign-users-and-groups-to-the-application"></a>将用户和组分配给应用程序

使用以下属性将用户分配给应用程序。

| 属性  | 说明 |ID  |
|---------|---------|---------|
| principalId | 将分配给应用程序的用户的用户 ID | 2fe96d23-5dc6-4f35-8222-0426a8c115c8 |
| principalType | 用户类型 | User |
| appRoleId |  应用程序的默认应用程序角色的应用程序角色 ID | 18d14569-c3bd-439b-9a66-3a2aee01d14f |
| resourceId | 应用程序的 servicePrincipal ID | b00c693f-9658-4c06-bd1b-c402c4653dea |

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/b00c693f-9658-4c06-bd1b-c402c4653dea/appRoleAssignments

Content-type: appRoleAssignments/json

{
  "principalId": "2fe96d23-5dc6-4f35-8222-0426a8c115c8",
  "principalType": "User",
  "appRoleId":"18d14569-c3bd-439b-9a66-3a2aee01d14f",
  "resourceId":"b00c693f-9658-4c06-bd1b-c402c4653dea"
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
    "resourceId": "b00c693f-9658-4c06-bd1b-c402c4653dea"
}
```

有关详细信息，请参阅[appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-beta)资源类型。



## <a name="additional-steps"></a>其他步骤
- [使用 PowerShell 示例为应用程序代理自动执行配置](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-powershell-samples.md)
- [使用 Microsoft Graph API 自动执行基于 SAML 的 SSO 应用配置](https://docs.microsoft.com/azure/active-directory/manage-apps/application-saml-sso-configure-api.md)
