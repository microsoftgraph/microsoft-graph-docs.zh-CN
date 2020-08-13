---
title: 使用 Microsoft Graph API 配置基于 SAML 的单一登录
description: 了解如何通过使用 Microsoft Graph API 来自动配置基于 SAML 的单一登录来节省时间。
author: kenwith
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.custom: scenarios:getting-started
ms.openlocfilehash: edc69453401a72242b01721d570cbf942bbf815d
ms.sourcegitcommit: 7dcd32f9e959bea2dfd81d9e0d4092f93da43cb7
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2020
ms.locfileid: "46658118"
---
# <a name="automate-saml-based-sso-app-configuration-with-microsoft-graph-api"></a>使用 Microsoft Graph API 自动化基于 SAML 的 SSO 应用配置

在本文中，您将学习如何从 Azure Active Directory（Azure AD）库中创建和配置应用程序。 本文使用 AWS 作为示例，但可以针对 Azure AD 库中的任何基于 SAML 的应用使用本文中的步骤。

**使用 Microsoft Graph API 来自动配置基于 SAML 的单一登录的步骤**

| 步骤  | 详细信息  |
|---------|---------|
| [1. 创建库应用程序](#step-1-create-the-gallery-application) | 登录到 API 客户端 <br> 检索库应用 <br> 创建库应用程序|
| [2. 配置单一登录](#step-2-configure-single-sign-on) | 检索应用对象 ID 和服务主体对象 ID <br> 设置单一登录模式 <br> 设置基本 SAML URL、例如标识符、回复 URL、登录 URL <br> 添加应用程序角色（可选）|
| [3. 配置声明映射](#step-3-configure-claims-mapping) | 创建声明映射策略 <br> 向服务主体分配声明映射策略|
| [4. 配置签名证书](#step-4-configure-signing-certificate) | 创建证书 <BR> 添加自定义签名密钥 <br> 激活自定义签名密钥|
| [5. 分配用户](#step-5-assign-users) | 向应用程序分配用户和组
| [6. 配置应用程序端](#step-6-configure-the-application-side)| 获取 Azure AD SAML 元数据

**文章中使用的所有 API 列表**

请确保你具有相应的权限来调用以下 API。

|资源类型 |方法 |
|---------|---------|
|[applicationTemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta)|[列出 applicationTemplate](https://docs.microsoft.com/graph/api/applicationtemplate-list?view=graph-rest-beta&tabs=http) <br>[实例化 applicationTemplate](https://docs.microsoft.com/graph/api/applicationtemplate-instantiate?view=graph-rest-beta&tabs=http)|
|[servicePrincipals](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)|[更新 servicePrincipal](https://docs.microsoft.com/graph/api/serviceprincipal-update?view=graph-rest-1.0&tabs=http) <br> [创建 appRoleAssignments](https://docs.microsoft.com/graph/api/serviceprincipal-post-approleassignments?view=graph-rest-1.0&tabs=http) <br> [分配 claimsMappingPolicies](https://docs.microsoft.com/graph/api/serviceprincipal-post-claimsmappingpolicies?view=graph-rest-beta&tabs=http)|
|[applications](https://docs.microsoft.com/graph/api/resources/application?view=graph-rest-1.0)|[更新应用程序](https://docs.microsoft.com/graph/api/application-update?view=graph-rest-1.0&tabs=http)|
|[claimsMappingPolicy](https://docs.microsoft.com/graph/api/resources/claimsmappingpolicy?view=graph-rest-beta)| [创建 claimsMappingPolicy](https://docs.microsoft.com/graph/api/claimsmappingpolicy-post-claimsmappingpolicies?view=graph-rest-beta&tabs=http)

>[!NOTE]
>本文中所示的响应对象可能会被缩短以提高可读性。 所有属性都是从实际调用返回。

## <a name="step-1-create-the-gallery-application"></a>第 1 步：创建库应用程序

### <a name="sign-in-to-microsoft-graph-explorer-recommended-postman-or-any-other-api-client-you-use"></a>登录到 Microsoft Graph Explorer（推荐），Postman 或使用的任何其他 API 客户端

1. 启动 [Microsoft Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)。
2. 选择**使用 Microsoft 登录**，然后使用 Azure AD 全局管理员或 App Admin 凭据登录。
3. 成功登录后，将在左侧窗格中看到用户帐户详细信息。

### <a name="retrieve-the-gallery-application-template-identifier"></a>检索库应用程序模板标识符

Azure AD 应用程序库中的每个应用程序都有一个[应用程序模板](https://docs.microsoft.com/graph/api/applicationtemplate-list?view=graph-rest-beta&tabs=http)，用于描述该应用程序的元数据。 使用此模板，可以在租户中创建应用程序和服务主体的实例以进行管理。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplates"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applicationTemplates
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationtemplates-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationtemplates-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationtemplates-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
  {
    "id": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "displayName": "Amazon Web Services (AWS)",
        "homePageUrl": "http://aws.amazon.com/",
        "supportedSingleSignOnModes": [
             "password",
             "saml",
             "external"
         ],
         "supportedProvisioningTypes": [
             "sync"
         ],
         "logoUrl": "https://az495088.vo.msecnd.net/app-logo/aws_215.png",
         "categories": [
             "developerServices"
         ],
         "publisher": "Amazon",
         "description": null    
  
}
```

### <a name="create-the-gallery-application"></a>创建库应用程序

使用在上一步中为应用程序检索的模板ID，在租户中为应用和服务主题[创建实例](https://docs.microsoft.com/graph/api/applicationtemplate-instantiate?view=graph-rest-beta&tabs=http)。

> [!NOTE] 
> 可以使用 applicationTemplate API 实例化[非库应用程序](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal)。 使用 applicationTemplateId `8adf8e6e-67b2-4cf2-a259-e3dc5476c621`。

> [!NOTE]
> 留出一些时间将应用程序配置到 Azure AD 租户中。 这不是即时的。 一种策略是每 5-10秒 对应用程序/服务主体对象执行 GET 查询，直到查询成功。


#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "applicationtemplate_instantiate"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/applicationTemplates/8b1025e4-1dd2-430b-a150-2ef79cd700f5/instantiate
Content-type: application/json

{
  "displayName": "AWS Contoso"
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

---


#### <a name="response"></a>响应


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationServicePrincipal"
} -->

```http
HTTP/1.1 201 OK
Content-type: application/json


{
    "application": {
        "objectId": "cbc071a6-0fa5-4859-8g55-e983ef63df63",
        "appId": "92653dd4-aa3a-3323-80cf-e8cfefcc8d5d",
        "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "displayName": "AWS Contoso",
        "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
        "replyUrls": [
            "https://signin.aws.amazon.com/saml"
        ],
        "logoutUrl": null,
        "samlMetadataUrl": null,
    },
    "servicePrincipal": {
        "objectId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e",
        "appDisplayName": "AWS Contoso",
        "applicationTemplateId": "8b1025e4-1dd2-430b-a150-2ef79cd700f5",
        "appRoleAssignmentRequired": true,
        "displayName": "My custom name",
        "homepage": "https://signin.aws.amazon.com/saml?metadata=aws|ISV9.1|primary|z",
        "replyUrls": [
            "https://signin.aws.amazon.com/saml"
        ],
        "servicePrincipalNames": [
            "93653dd4-aa3a-4323-80cf-e8cfefcc8d7d"
        ],
        "tags": [
            "WindowsAzureActiveDirectoryIntegratedApp"
        ],
    }
}
```

## <a name="step-2-configure-single-sign-on"></a>第 2 步：配置单一登录

### <a name="retrieve-app-object-id-and-service-principal-object-id"></a>检索应用对象 ID 和服务主体对象 ID

使用上一次调用的响应检索并保存应用程序对象 ID 和服务主体对象 ID。

```
"application": {
        "objectId": "cbc071a6-0fa5-4859-8g55-e983ef63df63"
}
"servicePrincipal": {
        "objectId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```
### <a name="set-single-sign-on-mode"></a>设置单一登录模式

在此示例中，将在 [ servicePrincipal 资源类型](https://docs.microsoft.com/graph/api/resources/serviceprincipal?view=graph-rest-1.0)中将 `saml` 设置为单一登录模式。 可以配置的其他 SAML SSO 属性是：`notificationEmailAddresses`、`loginUrl`、和 `samlSingleSignOnSettings.relayState`。

在此查询生效之前，需要在 Graph Explorer 中的**修改权限**选项卡上表示同意。 另外，请确保你使用的是先前获得的 **servicePrincipal** ID。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e
Content-type: servicePrincipal/json

{
    "preferredSingleSignOnMode": "saml"
}
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
HTTP/1.1 204
```

### <a name="set-basic-saml-urls-such-as-identifier-reply-url-sign-on-url"></a>设置基本 SAML URL、例如标识符、回复 URL、登录 URL

在应用程序对象中设置 AWS 的标识符并回复 URL。

请确保你使用的是之前获取的 **application** id。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/applications/cbc071a6-0fa5-4859-8g55-e983ef63df63
Content-type: applications/json

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
HTTP/1.1 204
```
### <a name="add-app-roles-optional"></a>添加应用程序角色（可选）

如果应用程序需要令牌中的角色信息，请在应用程序对象中添加角色的定义。 对于 AWS，可以[启用用户配置](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api)以从该 AWS 账户获取所有角色。 

有关详细信息，请参阅[配置 SAML 令牌中颁发的角色声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)。

> [!NOTE] 
> 添加应用程序角色时，请勿修改默认应用程序角色 msiam_access。 

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
PATCH https://graph.microsoft.com/beta/serviceprincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e
Content-type: serviceprincipals/json

{
"appRoles": [
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "msiam_access",
            "displayName": "msiam_access",
            "id": "7dfd756e-8c27-4472-b2b7-38c17fc5de5e",
            "isEnabled": true,
            "origin": "Application",
            "value": null
        },
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "Admin,WAAD",
            "displayName": "Admin,WAAD",
            "id": "454dc4c2-8176-498e-99df-8c4efcde41ef",
            "isEnabled": true,
            "value": "arn:aws:iam::212743507312:role/accountname-aws-admin,arn:aws:iam::212743507312:saml-provider/WAAD"
        },
        {
            "allowedMemberTypes": [
                "User"
            ],
            "description": "Finance,WAAD",
            "displayName": "Finance,WAAD",
            "id": "8642d5fa-18a3-4245-ab8c-a96000c1a217",
            "isEnabled": true,
            "value": "arn:aws:iam::212743507312:role/accountname-aws-finance,arn:aws:iam::212743507312:saml-provider/WAAD"
        }
    ]

}
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
HTTP/1.1 204
```

## <a name="step-3-configure-claims-mapping"></a>第 3 步：配置声明映射

### <a name="create-claims-mapping-policy"></a>创建声明映射策略

除了基本声明之外，还为 Azure AD 配置以下声明以在 SAML 令牌中发出：

| 声明名称 | 源  |
|---------|---------|
| `https://aws.amazon.com/SAML/Attributes/Role` | assignedroles| 
| `https://aws.amazon.com/SAML/Attributes/RoleSessionName` | userprincipalname |
| `https://aws.amazon.com/SAML/Attributes/SessionDuration` | "900" |
| roles | assignedroles |
| `http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier` | userprincipalname |

有关更多信息，请参阅[自定义令牌中发出的声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)。

> [!NOTE]
> 声明映射策略中的某些项区分大小写（例如“Version”）。 如果收到错误消息，例如“属性的值无效”，则可能是区分大小写的问题。

#### <a name="request"></a>请求


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->

```msgraph-interactive
POST https://graph.microsoft.com/beta/policies/claimsMappingPolicies
Content-type: claimsMappingPolicies/json

{
    "definition":[
            "{\"ClaimsMappingPolicy\": {
                \"Version\": 1,
                \"IncludeBasicClaimSet\": \"true\",
                \"ClaimsSchema\": [
                    {
                        \"Source\": \"user\",
                        \"ID\": \"assignedroles\",
                        \"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/Role\"
                    },
                    {
                        \"Source\": \"user\",
                        \"ID\": \"userprincipalname\",
                        \"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"
                    },
                    {
                        \"Source\": \"user\",
                        \"ID\": \"900\",
                        \"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"
                    },
                    {
                        \"Source\": \"user\",
                        \"ID\": \"assignedroles\",
                        \"SamlClaimType\": \"appRoles\"
                    },
                    {
                        \"Source\": \"user\",
                        \"ID\": \"userprincipalname\",
                        \"SamlClaimType\": \"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"
                    }
                ]
            }
        }"

    ],
    "displayName": "AWS Claims policy",
    "isOrganizationDefault": false
}
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
  "@odata.type": "microsoft.graph.claimsMappingPolicies",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: claimsMappingPolicies/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#policies/claimsMappingPolicies/$entity",
    "id": "6b33aa8e-51f3-41a6-a0fd-d660d276197a",
    "definition": [
        "{\"ClaimsMappingPolicy\": {\"Version\": 1,\"IncludeBasicClaimSet\": \"true\",\"ClaimsSchema\": [{\"Source\": \"user\",\"ID\": \"assignedroles\",\"SamlClaimType\":\"https://aws.amazon.com/SAML/Attributes/Role\"\r\n                    },{\"Source\": \"user\",\"ID\": \"userprincipalname\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/RoleSessionName\"},{\"Source\": \"user\",\"ID\": \"900\",\"SamlClaimType\": \"https://aws.amazon.com/SAML/Attributes/SessionDuration\"},{\"Source\": \"user\",\"ID\": \"assignedroles\",\"SamlClaimType\":\"appRoles\"},{\"Source\": \"user\",\"ID\": \"userprincipalname\",\"SamlClaimType\": \"http://schemas.xmlsoap.org/ws/2005/05/identity/claims/nameidentifier\"}]}}"
    ],
    "displayName": "AWS Claims policy",
    "isOrganizationDefault": false
}
```

### <a name="assign-claims-mapping-policy-to-service-principal"></a>向服务主体分配声明映射策略

#### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/beta/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e/claimsMappingPolicies/$ref

Content-type: claimsMappingPolicies/json

{
  "@odata.id":"https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/6b33aa8e-51f3-41a6-a0fd-d660d276197a"
}
```


#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

## <a name="step-4-configure-signing-certificate"></a>第 4 步：配置签名证书

默认情况下，使用 [applicationTemplate](https://docs.microsoft.com/graph/api/resources/applicationtemplate?view=graph-rest-beta) API 无法创建签名证书。 创建自定义签名证书并将其分配给应用程序。 

### <a name="create-a-custom-signing-certificate"></a>创建自定义签名证书

要进行测试，可以使用以下 PowerShell 命令获取自签名证书。 然后需要使用其他工具手动操作和提取所需的值。 使用公司的最佳安全实践，创建用于生产的签名证书。

```powershell
Param(
    [Parameter(Mandatory=$true)]
    [string]$fqdn,
    [Parameter(Mandatory=$true)]
    [string]$pwd,
    [Parameter(Mandatory=$true)]
    [string]$location
) 

if (!$PSBoundParameters.ContainsKey('location'))
{
    $location = "."
} 

$cert = New-SelfSignedCertificate -certstorelocation cert:\currentuser\my -DnsName $fqdn
$pwdSecure = ConvertTo-SecureString -String $pwd -Force -AsPlainText
$path = 'cert:\currentuser\my\' + $cert.Thumbprint
$cerFile = $location + "\\" + $fqdn + ".cer"
$pfxFile = $location + "\\" + $fqdn + ".pfx" 

Export-PfxCertificate -cert $path -FilePath $pfxFile -Password $pwdSecure
Export-Certificate -cert $path -FilePath $cerFile
```

或者，可以将以下 C# 控制台应用程序用作概念证明，以了解如何获取所需的值。 请注意，该代码仅用于**学习和参考**，不应在生产中直接使用。

```csharp
using System;
using System.Security.Cryptography;
using System.Security.Cryptography.X509Certificates;
using System.Text;


/* CONSOLE APP - PROOF OF CONCEPT CODE ONLY!!
 * This code uses a self signed certificate and should not be used 
 * in production. This code is for reference and learning ONLY.
 */
namespace Self_signed_cert
{
    class Program
    {
        static void Main(string[] args)
        {
            // Generate a guid to use as a password and then create the cert.
            string password = Guid.NewGuid().ToString();
            var selfsignedCert = buildSelfSignedServerCertificate(password);

            // Print values so we can copy paste into the JSON fields.
            // Print out the private key in base64 format.
            Console.WriteLine("Private Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Pfx, password)), Environment.NewLine);

            // Print out the start date in ISO 8601 format.
            DateTime startDate = DateTime.Parse(selfsignedCert.GetEffectiveDateString()).ToUniversalTime();
            Console.WriteLine("For All startDateTime: " + startDate.ToString("o"));

            // Print out the end date in ISO 8601 format.
            DateTime endDate = DateTime.Parse(selfsignedCert.GetExpirationDateString()).ToUniversalTime();
            Console.WriteLine("For All endDateTime: " + endDate.ToString("o"));

            // Print the GUID used for keyId
            string signAndPasswordGuid = Guid.NewGuid().ToString();
            string verifyGuid = Guid.NewGuid().ToString();
            Console.WriteLine("GUID to use for keyId for keyCredentials->Usage == Sign and passwordCredentials: " + signAndPasswordGuid);
            Console.WriteLine("GUID to use for keyId for keyCredentials->Usage == Verify: " + verifyGuid);

            // Print out the password.
            Console.WriteLine("Password is: {0}", password);

            // Print out a displayName to use as an example.
            Console.WriteLine("displayName to use: CN=Example");
            Console.WriteLine();

            // Print out the public key.
            Console.WriteLine("Public Key: {0}{1}", Convert.ToBase64String(selfsignedCert.Export(X509ContentType.Cert)), Environment.NewLine);
            Console.WriteLine();

            // Generate the customKeyIdentifier using hash of thumbprint.
            Console.WriteLine("You can generate the customKeyIdentifier by getting the SHA256 hash of the certs thumprint.\nThe certs thumbprint is: {0}{1}", selfsignedCert.Thumbprint, Environment.NewLine);
            Console.WriteLine("The hash of the thumbprint that we will use for customeKeyIdentifier is:");
            string keyIdentifier = GetSha256FromThumbprint(selfsignedCert.Thumbprint);
            Console.WriteLine(keyIdentifier);
        }

        // Generate a self-signed certificate.
        private static X509Certificate2 buildSelfSignedServerCertificate(string password)
        {
            const string CertificateName = @"Microsoft Azure Federated SSO Certificate TEST";
            DateTime certificateStartDate = DateTime.UtcNow;
            DateTime certificateEndDate = certificateStartDate.AddYears(2).ToUniversalTime();

            X500DistinguishedName distinguishedName = new X500DistinguishedName($"CN={CertificateName}");

            using (RSA rsa = RSA.Create(2048))
            {
                var request = new CertificateRequest(distinguishedName, rsa, HashAlgorithmName.SHA256, RSASignaturePadding.Pkcs1);

                request.CertificateExtensions.Add(
                    new X509KeyUsageExtension(X509KeyUsageFlags.DataEncipherment | X509KeyUsageFlags.KeyEncipherment | X509KeyUsageFlags.DigitalSignature, false));

                var certificate = request.CreateSelfSigned(new DateTimeOffset(certificateStartDate), new DateTimeOffset(certificateEndDate));
                certificate.FriendlyName = CertificateName;

                return new X509Certificate2(certificate.Export(X509ContentType.Pfx, password), password, X509KeyStorageFlags.Exportable);
            }
        }

        // Generate hash from thumbprint.
        public static string GetSha256FromThumbprint(string thumbprint)
        {
            var message = Encoding.ASCII.GetBytes(thumbprint);
            SHA256Managed hashString = new SHA256Managed();
            return Convert.ToBase64String(hashString.ComputeHash(message));
        }
    }
}
```

### <a name="add-a-custom-signing-key"></a>添加自定义签名密钥

向服务主体添加以下信息：

* 私钥
* 密码
* 公钥 

从PFX文件中提取 Base64 编码公钥和私钥。 要了解有关属性的更多信息，请参阅 [keyCredential 资源类型](https://docs.microsoft.com/graph/api/resources/keycredential?view=graph-rest-1.0)。

确保用于“签名”的 keyCredential 的keyId 与 passwordCredential 的 keyId 相匹配。 可以通过获取证书指纹的哈希值来生成 `customkeyIdentifier`。 请参阅前面的 C# 参考代码。

#### <a name="request"></a>请求

> [!NOTE]
> 为了提高可读性，keyCredentials 属性中的“项”值被缩短。 该值为 base 64 编码。 对于私钥，属性 `usage` 是“签名”。 对于公钥，属性 `usage` 是“验证”。

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e

Content-type: servicePrincipals/json

{
    "keyCredentials":[
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "endDateTime": "2021-04-22T22:10:13Z",
            "keyId": "4c266507-3e74-4b91-aeba-18a25b450f6e",
            "startDateTime": "2020-04-22T21:50:13Z",
            "type": "X509CertAndPassword",
            "usage": "Sign",
            "key":"MIIKIAIBAz.....HBgUrDgMCERE20nuTptI9MEFCh2Ih2jaaLZBZGeZBRFVNXeZmAAgIH0A==",
            "displayName": "CN=awsAPI"
        },
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "endDateTime": "2021-04-22T22:10:13Z",
            "keyId": "e35a7d11-fef0-49ad-9f3e-aacbe0a42c42",
            "startDateTime": "2020-04-22T21:50:13Z",
            "type": "AsymmetricX509Cert",
            "usage": "Verify",
            "key": "MIIDJzCCAg+gAw......CTxQvJ/zN3bafeesMSueR83hlCSyg==",
            "displayName": "CN=awsAPI"
        }

    ],
    "passwordCredentials": [
        {
            "customKeyIdentifier": "lY85bR8r6yWTW6jnciNEONwlVhDyiQjdVLgPDnkI5mA=",
            "keyId": "4c266507-3e74-4b91-aeba-18a25b450f6e",
            "endDateTime": "2022-01-27T19:40:33Z",
            "startDateTime": "2020-04-20T19:40:33Z",
            "secretText": "61891f4ee44d"
        }
    ]
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```

### <a name="activate-the-custom-signing-key"></a>激活自定义签名密钥

需要将 `preferredTokenSigningKeyThumbprint` 属性设置为想要 Azure AD 用于签署 SAML 响应的证书的指纹。 

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e

Content-type: servicePrincipals/json

{
    "preferredTokenSigningKeyThumbprint": "AC09FEF18DDE6983EE2A164FBA3C4DD7518BD787"
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 204
```
## <a name="step-5-assign-users"></a>第 5 步：分配用户

### <a name="assign-users-and-groups-to-the-application"></a>向应用程序分配用户和组

将以下用户分配给服务主体，然后分配 AWS_Role1。 

| 名称  | ID  |
|---------|---------|
| 用户 ID （principalId） | 6cad4079-4e79-4a3f-9efb-ea30a14bdb26 |
| 类型（PrincipalType） | 用户 |
| 应用程序角色 ID （appRoleId） | 454dc4c2-8176-498e-99df-8c4efcde41ef |
| servicePrincipalID (resourceId) | f47a6776-bca7-4f2e-bc6c-eec59d058e3e |

#### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "servicePrincipals"
}-->
```msgraph-interactive
POST https://graph.microsoft.com/v1.0/servicePrincipals/f47a6776-bca7-4f2e-bc6c-eec59d058e3e/appRoleAssignments

Content-type: appRoleAssignments/json

{
  "principalId": "6cad4079-4e79-4a3f-9efb-ea30a14bdb26",
  "principalType": "User",
  "appRoleId":"454dc4c2-8176-498e-99df-8c4efcde41ef",
  "resourceId":"f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true,
} -->
```http
HTTP/1.1 201 
Content-type: appRoleAssignments/json

{
    "id": "rq7hyzl4yECaNZleMrTpDV-OCe5TEl5Ao_o76XMrRFU",
    "creationTimestamp": "2020-04-23T17:38:13.2508567Z",
    "appRoleId": "454dc4c2-8176-498e-99df-8c4efcde41ef",
    "principalDisplayName": "User 1",
    "principalId": "6cad4079-4e79-4a3f-9efb-ea30a14bdb26",
    "principalType": "User",
    "resourceDisplayName": "AWS API Created",
    "resourceId": "f47a6776-bca7-4f2e-bc6c-eec59d058e3e"
}
```

有关详细信息，请参阅 [appRoleAssignment](https://docs.microsoft.com/graph/api/resources/approleassignment?view=graph-rest-1.0)。

## <a name="step-6-configure-the-application-side"></a>第 6 步：配置应用程序端

### <a name="get-azure-ad-saml-metadata"></a>获取 Azure AD SAML 元数据

使用以下 URL 获取特定配置的应用程序的 Azure AD SAML 元数据。 元数据包含诸如签名证书、Azure AD entityID和 Azure AD SingleSignOnService 等信息。

`https://login.microsoftonline.com/{tenant-id}/federationmetadata/2007-06/federationmetadata.xml?appid={app-id}`

## <a name="next-steps"></a>后续步骤
- [使用 Microsoft Graph API 配置用户预配](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-configure-api)
- [使用 AD FS 应用程序活动报告将应用程序迁移到 Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-application-activity)
