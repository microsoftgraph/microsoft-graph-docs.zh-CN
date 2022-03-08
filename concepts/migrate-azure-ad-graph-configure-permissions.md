---
title: 配置Azure AD Graph注册所需的权限
description: 配置Azure AD Graph注册所需的权限。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: fa74def34e93bed88513e564931a5b6557ed1bc8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334987"
---
# <a name="configure-required-azure-ad-graph-permissions-for-an-app-registration"></a>配置Azure AD Graph注册所需的权限

Azure Active Directory (Azure AD) Graph弃用，并将于近期停用。 作为此弃用路径的一Azure AD Graph，现已禁用通过 Azure 门户向应用注册添加权限。 我们建议你遵循应用迁移[规划清单](migrate-azure-ad-graph-planning-checklist.md)来帮助你将应用转换为 [Microsoft](/graph/overview) Graph API。

但是，你的应用可能仍临时Azure AD Graph访问资源的权限。 本文介绍了以下四种用于配置应用注册Azure AD Graph权限的方法：

1. [使用 Azure 门户查找组织使用的 API](#option-1-use-the-azure-portal-to-find-the-apis-your-organization-uses)
1. [更新 Azure 门户上的应用程序清单](#option-2-update-the-application-manifest-on-the-azure-portal)
1. [使用 Microsoft Graph API](#option-3-use-the-microsoft-graph-api)
1. [使用 Microsoft Graph PowerShell SDK](#option-4-use-the-microsoft-graph-powershell-sdk)

> [!CAUTION]
> 任何使用 Azure AD Graph 的应用在 API 停用后Azure AD Graph运行。 有关详细信息，请参阅将Azure AD Graph[迁移到 Microsoft Graph](migrate-azure-ad-graph-overview.md)。

## <a name="option-1-use-the-azure-portal-to-find-the-apis-your-organization-uses"></a>选项 1：使用 Azure 门户查找组织使用的 API

1. 以全局管理员或应用程序管理员登录 [Azure](https://portal.azure.com) 门户。
1. 搜索并选择"Azure Active Directory **"**。
1. 在“**管理**”之下，选择“**应用注册**”。
1. 在 **"应用注册"** 窗口的"所有应用程序"选项卡下，选择要添加其权限Azure AD Graph应用。 这将打开应用注册的 **"概述"** 窗格。
1. 从窗口的左侧窗格的"管理"菜单组下，选择 **"API 权限"**。 这将显示 **应用注册** 的已配置权限。 选择“**添加权限**”。
1. 在显示 **的请求 API** 权限窗口中，切换到我的组织使用的 API 选项卡并搜索  `Windows Azure Active Directory` 或 。`00000002-0000-0000-c000-000000000000` 从筛选列表中选择以显示 **"Azure Active Directory Graph权限**"窗口。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AzureADGraphPermissionsAPI.png" alt-text="Azure AD Graph API 由 Windows Azure Active Directory 和 clientID 00000002-0000-0000-c000-000000000000 标识。" border="true":::

1. 选择 **"委派权限"** 或" **应用程序权限"** 选项卡，分别从委派权限和应用程序权限中选择。 选择 **"添加权限** "，将权限添加到应用注册。
1. 添加所需的权限后，返回到"配置的权限"窗口中，选择"授予管理员同意Azure AD Graph应用注册的权限。

## <a name="option-2-update-the-application-manifest-on-the-azure-portal"></a>选项 2：更新 Azure 门户上的应用程序清单

1. 以全局管理员或应用程序管理员登录 [Azure](https://portal.azure.com) 门户。
1. 搜索并选择"Azure Active Directory **"**。
1. 在“**管理**”之下，选择“**应用注册**”。
1. 在 **"应用注册"** 窗口的"所有应用程序"选项卡下，选择要添加其权限Azure AD Graph应用。 这将打开应用注册的 **"概述"** 窗格。
1. 从窗口的左侧窗格的"管理"菜单组下，选择"清单 **"**。 这将打开一个编辑器，允许你直接编辑应用注册对象的属性。

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppRegistrationManifest.png" alt-text="应用注册清单文件允许你编辑应用程序的属性。" border="true":::

1. 在应用的清单文件中仔细编辑 **requiredResourceAccess** 属性，以添加以下详细信息：
    >**注意：** 可以在 Azure 门户上编辑应用清单或选择"下载"以在本地编辑清单，Upload将其重新应用至应用程序。
+ 添加 **resourceAppId** 属性并分配代表 `00000002-0000-0000-c000-000000000000` Azure AD Graph
+ 添加 **resourceAccess** 属性并分配所需的权限。

    以下 JSON 代码段显示具有 Azure AD Graph 作为资源的 **requiredResourceAccess** 属性，并分别为 *User.Read* 和 *Application.Read.All* oauth2PermissionScope (委派权限) 和 appRole (应用程序权限) 。    

    ```JSON
    "requiredResourceAccess": [
        {
            "resourceAppId": "00000002-0000-0000-c000-000000000000",
            "resourceAccess": [
                {
                    "id": "311a71cc-e848-46a1-bdf8-97ff7156d8e6",
                    "type": "Scope"
                },
                {
                    "id": "3afa6a7d-9b1a-42eb-948e-1650a849e176",
                    "type": "Role"
                }
            ]
        }
    ],
    ```

7. 保存所做的更改。
8. 选择 **"API 权限"**，在"为应用注册配置的权限"中，选择"授予管理员同意"以向Azure AD Graph授予应用注册权限。

## <a name="option-3-use-the-microsoft-graph-api"></a>选项 3：使用 Microsoft Graph API

Microsoft Graph [应用程序](/graph/api/resources/application) API 包含 **requiredResourceAccess** 属性，该属性是 [requiredResourceAccess 对象](/graph/api/resources/requiredresourceaccess)的集合。 使用此属性配置所需的Azure AD Graph权限，如以下步骤所述。

### <a name="prerequisites"></a>先决条件

若要完成以下步骤，您需要以下资源和权限：

+ 在自己选择的工具中运行 HTTP 请求，例如，在应用中，通过 Graph [资源管理器](https://aka.ms/ge)或 Postman。
+ 以全局管理员或应用程序管理员角色中的用户或目标应用注册的所有者运行 API。 有关这些角色支持的操作详细信息，请参阅Azure AD[角色](/azure/active-directory/roles/permissions-reference)。
+ 必须授予用于进行这些更改的应用的权限 `Application.ReadWrite.All` 。

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>步骤 1：确定应用Azure AD Graph权限的权限标识

确定Azure AD Graph所需的权限、其权限标识，以及它们是否是应用程序角色 (应用程序权限) 或 oauth2PermissionScopes (委派) 。

Azure AD Graph标识为 servicePrincipal `00000002-0000-0000-c000-000000000000` 对象，该对象的全局唯一 appId `Windows Azure Active Directory` 及其 **displayName** 和 **appDisplayName**。 运行以下请求以检索服务主体对象Azure AD Graph。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "migrate-azureadgraph-get-serviceprincipal-azureadgraph"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/servicePrincipals?$filter=appId eq '00000002-0000-0000-c000-000000000000'
```

#### <a name="response"></a>响应

在响应对象中，Azure AD Graph应用程序权限的详细信息列在 **appRoles** 对象中，而委派权限的详细信息列在 **oauth2PermissionScopes** 对象中。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals",
    "value": [
        {
            "id": "1804a6f8-e623-4520-8f40-ba1b0c11c42d",
            "accountEnabled": true,
            "appDisplayName": "Windows Azure Active Directory",
            "appDescription": null,
            "appId": "00000002-0000-0000-c000-000000000000",
            "appOwnerOrganizationId": "f8cdef31-a31e-4b4a-93e4-5f571e91255a",
            "appRoleAssignmentRequired": false,
            "displayName": "Windows Azure Active Directory",
            "servicePrincipalNames": [
                "https://graph.windows.net",
                "00000002-0000-0000-c000-000000000000/graph.microsoftazure.us",
                "00000002-0000-0000-c000-000000000000/graph.windows.net",
                "00000002-0000-0000-c000-000000000000/directory.windows.net",
                "00000002-0000-0000-c000-000000000000",
                "https://graph.windows.net/",
                "https://graph.microsoftazure.us"
            ],
            "servicePrincipalType": "Application",
            "signInAudience": "AzureADMultipleOrgs",
            "appRoles": [
                {
                    "allowedMemberTypes": [
                        "Application"
                    ],
                    "description": "Allows the app to read applications and service principals without a signed-in user",
                    "displayName": "Read all applications",
                    "id": "3afa6a7d-9b1a-42eb-948e-1650a849e176",
                    "isEnabled": true,
                    "origin": "Application",
                    "value": "Application.Read.All"
                }
            ],
            "oauth2PermissionScopes": [
                {
                    "adminConsentDescription": "Allows users to sign in to the app, and allows the app to read the profile of signed-in users. It also allow the app to read basic company information of signed-in users.",
                    "adminConsentDisplayName": "Sign in and read user profile",
                    "id": "311a71cc-e848-46a1-bdf8-97ff7156d8e6",
                    "isEnabled": true,
                    "type": "User",
                    "userConsentDescription": "Allows you to sign in to the app with your work account and let the app read your profile. It also allows the app to read basic company information.",
                    "userConsentDisplayName": "Sign you in and read your profile",
                    "value": "User.Read"
                }
            ]
        }
    ]
}
```

从上述截断的输出中， `311a71cc-e848-46a1-bdf8-97ff7156d8e6` 是 *User.Read* `3afa6a7d-9b1a-42eb-948e-1650a849e176` 委派权限的权限 ID，而 是 *Application.Read.All* 应用程序权限的权限 ID。

### <a name="step-2-add-required-azure-ad-graph-permissions-to-your-app"></a>步骤 2：将Azure AD Graph权限添加到应用

以下示例调用[更新](/graph/api/application-update)应用程序 API，以将Azure AD Graph应用程序注册所需的权限添加到对象 ID 标识的应用注册`581088ba-83c5-4975-b8af-11d2d7a76e98`。 在步骤 1 中，这些权限分别为 *User.Read* 和 *Application.Read.All* 委派权限和应用程序权限。

> [!IMPORTANT]
> 若要更新 **requiredResourceAccess** 属性，必须同时传递现有权限和新权限。 仅传递新权限会覆盖并删除现有权限。

#### <a name="request"></a>请求

<!-- {
  "blockType": "request",
  "name": "migrate-azureadgraph-update-application"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/applications/581088ba-83c5-4975-b8af-11d2d7a76e98
Content-Type: application/json

{
    "requiredResourceAccess": [
        {
            "resourceAppId": "00000002-0000-0000-c000-000000000000",
            "resourceAccess": [
                {
                    "id": "311a71cc-e848-46a1-bdf8-97ff7156d8e6",
                    "type": "Scope"
                },
                {
                    "id": "3afa6a7d-9b1a-42eb-948e-1650a849e176",
                    "type": "Role"
                }
            ]
        }
    ]
}
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

### <a name="step-3-verify-that-the-required-azure-ad-graph-permissions-were-added-to-your-app"></a>步骤 3：验证Azure AD Graph权限已添加到应用

通过使用 Microsoft Graph API 或检查 Azure 门户中的"应用注册"页面，验证应用注册是否具有在步骤 2 中添加的Azure AD Graph API 权限。

#### <a name="use-the-microsoft-graph-get-applicationid-api"></a>使用 Microsoft Graph GET /application/{id} API

以下请求检索由对象 ID 标识的应用的 **id** 和 **requiredResourceAccess** **属性**`581088ba-83c5-4975-b8af-11d2d7a76e98`。

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/581088ba-83c5-4975-b8af-11d2d7a76e98?$select=id,requiredResourceAccess
```

>**注意：** 虽然你已配置应用所需的权限，但是尚未授予这些权限。 许多权限都需要获得管理员同意，然后才能用于访问组织数据。

## <a name="option-4-use-the-microsoft-graph-powershell-sdk"></a>选项 4：使用 Microsoft Graph PowerShell SDK

Microsoft Graph PowerShell SDK 中的 [Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true) cmdlet 包括 **RequiredResourceAccess** 参数，该参数是 **IMicrosoftGraphRequiredResourceAccess** 对象的集合。 使用此参数配置所需的Azure AD Graph权限，如以下步骤所述。

### <a name="prerequisites"></a>先决条件

若要完成以下步骤，需要以下权限：

+ 身份验证的 PowerShell 会话 (，例如，使用 `Connect-MgGraph`) 。
+ Microsoft Graph PowerShell 必须被授予`Application.ReadWrite.All`权限。
+ 登录用户必须被授予全局管理员或应用程序管理员Azure AD目录角色，或者成为目标应用注册的所有者。 有关这些角色支持的操作详细信息，请参阅Azure AD[角色](/azure/active-directory/roles/permissions-reference)。

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>步骤 1：确定应用Azure AD Graph权限的权限标识

确定Azure AD Graph所需的权限、其权限标识，以及他们是应用程序角色 (应用程序权限) 委派权限。

Azure AD Graph标识为 ServicePrincipal `00000002-0000-0000-c000-000000000000` 对象，该对象的全局唯一 AppId `Windows Azure Active Directory` 及其 **DisplayName** 和 **AppDisplayName**。 运行以下请求以检索 ServicePrincipal 对象Azure AD Graph。

#### <a name="request"></a>请求

创建一个名为 **fetchPermissions.ps1的新** PowerShell 脚本并添加以下代码。 此代码检索Azure AD Graph和类型。 输出显示 **AppRoles** 和 **Oauth2PermissionScopes** 对象的输出并设置其格式。

```powershell
# Sign in with the required Application.ReadWrite.All scope
Connect-Graph -Scopes "Application.ReadWrite.All"

# Retrieve the service principal details for Azure AD Graph API.
$AADGraph = Get-MgServicePrincipal -Filter "appId eq '00000002-0000-0000-c000-000000000000'"

# Format output of the request above and display AppRoles (application permissions) and oauth2PermissionScopes (delegated permissions)
Echo "Azure AD Graph service principal object and its supported permissions:"
Echo "Application permissions:"
$AADGraph.AppRoles | Format-List
Echo "Delegated permissions:"
$AADGraph.Oauth2PermissionScopes | Format-List
```

运行以下命令的脚本
```powershell
.\fetchPermissions.ps1
```

#### <a name="response"></a>响应

下面是一个输出示例。

```powershell
Welcome To Microsoft Graph!
Azure AD Graph service principal object and its supported permissions:
Application permissions:


AllowedMemberTypes   : {Application}
Description          : Allows the app to read applications and service principals without a signed-in user
DisplayName          : Read all applications
Id                   : 3afa6a7d-9b1a-42eb-948e-1650a849e176
IsEnabled            : True
Origin               : Application
Value                : Application.Read.All
AdditionalProperties : {}

Delegated permissions:


AdminConsentDescription : Allows users to sign in to the app, and allows the app to read the profile of signed-in users. It also allow the app to read basic company information of signed-in users.
AdminConsentDisplayName : Sign in and read user profile
Id                      : 311a71cc-e848-46a1-bdf8-97ff7156d8e6
IsEnabled               : True
Origin                  :
Type                    : User
UserConsentDescription  : Allows you to sign in to the app with your work account and let the app read your profile. It also allows the app to read basic company information.
UserConsentDisplayName  : Sign you in and read your profile
Value                   : User.Read
AdditionalProperties    : {}
```

从此输出中， `311a71cc-e848-46a1-bdf8-97ff7156d8e6` 是 *User.Read* `3afa6a7d-9b1a-42eb-948e-1650a849e176` 委派权限的权限 ID，而 是 *Application.Read.All* 应用程序权限的权限 ID。

### <a name="step-2-add-azure-ad-graph-permissions-to-your-app"></a>步骤 2：Azure AD Graph应用程序添加权限

创建一个名为 **updatePermissions.ps1的新** PowerShell 脚本并添加以下代码。 此代码将所需的Azure AD Graph添加到对象 ID `581088ba-83c5-4975-b8af-11d2d7a76e98`标识的应用注册。 在步骤 1 中，这些权限分别为 *User.Read* 和 *Application.Read.All* 委派权限和应用程序权限。

> [!IMPORTANT]
> 若要更新 **RequiredResourceAccess** 属性，必须同时传递现有权限和新权限。 仅传递新权限会覆盖并删除现有权限。

#### <a name="request"></a>请求

```powershell
# Sign in with the required Application.ReadWrite.All scope
Connect-Graph -Scopes "Application.ReadWrite.All" 

## Replace 581088ba-83c5-4975-b8af-11d2d7a76e98 with the object ID of the app you wish to add new permissions to
$applicationId = '581088ba-83c5-4975-b8af-11d2d7a76e98' 

$app = Get-MgApplication -ApplicationId $applicationId

## Azure AD Graph's globally unique appId is 00000002-0000-0000-c000-000000000000 identified by the ResourceAppId
$aadAccess = $app.RequiredResourceAccess | Where-Object { $_.ResourceAppId -eq '00000002-0000-0000-c000-000000000000' } 

if($null -eq $aadAccess){ 
    $app.RequiredResourceAccess += @{  
        ResourceAppId = "00000002-0000-0000-c000-000000000000"; 
        ResourceAccess = @( 

                ## Replace the following with values of ID and type for all permissions - both new and existing permissions - you want to configure for the app
                @{ 
                    # User.Read delegated permission Sign in and read user profile 
                    id = "311a71cc-e848-46a1-bdf8-97ff7156d8e6";  
                    type = "Scope"; 
                }, 
                @{ 
                    # Application.Read.All app role (application permission) to view application data
                    id = "3afa6a7d-9b1a-42eb-948e-1650a849e176"; 
                    type = "Role"; 
                }
            ) 
     } 
} 

Update-MgApplication -ApplicationId $applicationId -RequiredResourceAccess $app.RequiredResourceAccess 
```

运行以下命令的脚本。
```powershell
.\updatePermissions.ps1
```

### <a name="response"></a>响应

下面是一个输出示例。

```powershell
Welcome To Microsoft Graph!
```

>**注意：** 虽然你已配置应用所需的权限，但是尚未授予这些权限。 许多权限都需要获得管理员同意，然后才能用于访问组织数据。

## <a name="see-also"></a>另请参阅

+ [应用程序 API](/graph/api/resources/application)
+ [Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true)
