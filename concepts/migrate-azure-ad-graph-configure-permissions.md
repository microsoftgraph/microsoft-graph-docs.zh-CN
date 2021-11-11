---
title: 使用 Microsoft Graph配置Azure AD Graph注册所需的权限
description: 使用 Microsoft Graph配置应用Azure AD Graph所需的权限。
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 25fac773056238bde7c50158eb09daf3f5080552
ms.sourcegitcommit: 6b5bee1a1cea92c1f3d6439110c4916eb8b249a5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/11/2021
ms.locfileid: "60908581"
---
# <a name="use-microsoft-graph-to-configure-required-azure-ad-graph-permissions-for-an-app-registration"></a>使用 Microsoft Graph配置Azure AD Graph注册所需的权限

Azure Active Directory (Azure AD) Graph弃用，将于 2022 年 6 月 30 日停用。 作为此弃用路径的一Azure AD Graph，现已禁用通过 Azure 门户向应用注册所需的权限添加权限。 我们建议你遵循应用[迁移规划清单](migrate-azure-ad-graph-planning-checklist.md)来帮助你将应用转换到[Microsoft](/graph/overview) Graph API。

但是，你可能需要向应用Azure AD Graph权限。 本文提供有关使用 Microsoft Graph配置应用注册Azure AD Graph权限的指南。

> [!CAUTION]
> 任何使用 Azure AD Graph的应用在 2022 年 6 月 30 日之后仍将停止运行。 有关详细信息，请参阅将Azure AD Graph[迁移到 Microsoft Graph。](migrate-azure-ad-graph-overview.md)

## <a name="option-1-use-the-microsoft-graph-api"></a>选项 1：使用 Microsoft Graph API

Microsoft Graph [应用程序](/graph/api/resources/application)API 包含 **requiredResourceAccess** 属性，该属性是 [requiredResourceAccess 对象](/graph/api/resources/requiredresourceaccess)的集合。 使用此属性可以配置Azure AD Graph权限，如以下步骤所述。

### <a name="prerequisites"></a>先决条件

若要完成以下步骤，您需要以下资源和权限：

+ 在所选择的工具中运行 HTTP 请求，例如在应用中，通过 Graph [Explorer](https://aka.ms/ge)或 Postman 运行。
+ 以全局管理员或应用程序管理员角色中的用户或目标应用注册的所有者运行 API。 有关这些角色支持的操作详细信息，请参阅Azure AD[角色](/azure/active-directory/roles/permissions-reference)。
+ 必须授予用于进行这些更改的应用 `Application.ReadWrite.All` 的权限。

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>步骤 1：确定应用Azure AD Graph权限的权限标识

确定Azure AD Graph所需的权限、其权限标识，以及它们是应用程序角色 (应用程序权限) 委派权限。 可以通过在 Azure 门户上的应用清单中读取其 **requiredResourceAccess** 属性，或者通过 Microsoft Graph API 从具有配置权限的现有应用注册中检索权限 ID。 

Azure AD Graph的全局唯一 **appId** 是 ，并且由 `00000002-0000-0000-c000-000000000000` **requiredResourceAccess** 属性的 **resourceAppId** 属性标识。

### <a name="request"></a>请求

以下请求从Azure AD Graph id 标识的现有应用程序中检索权限 ID 和 **类型** `f7748341-825c-46e9-a111-5e3b56ae015b` 。

<!-- {
  "blockType": "request",
  "name": "migrate-azureadgraph-get-serviceprincipal-azureadgraph"
}-->

```msgraph-interactive
https://graph.microsoft.com/v1.0/applications/f7748341-825c-46e9-a111-5e3b56ae015b?$select=requiredResourceAccess
```

### <a name="response"></a>响应

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#applications(requiredResourceAccess)/$entity",
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

在此输出中， `311a71cc-e848-46a1-bdf8-97ff7156d8e6` 是 *User.Read* 委派权限的权限 `3afa6a7d-9b1a-42eb-948e-1650a849e176` ID，而 是 *Application.Read.All* 应用程序角色的权限 ID。

### <a name="step-2-add-required-azure-ad-graph-permissions-to-your-app"></a>步骤 2：将Azure AD Graph权限添加到应用

以下示例调用[更新](/graph/api/application-update)应用程序 API，以将Azure AD Graph应用程序注册所需的权限添加到对象 ID 标识的应用注册 `581088ba-83c5-4975-b8af-11d2d7a76e98` 中。 在步骤 1 中，这些权限分别为 *User.Read* 和 *Application.Read.All* 委派权限和应用程序角色。

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

通过使用 Microsoft Graph API 或检查 Azure 门户中的"应用注册"页面，验证应用注册是否具有在步骤 2 中添加的必需 API 权限。 

#### <a name="use-the-microsoft-graph-get-applicationid-api"></a>使用 Microsoft Graph GET /application/{id} API

以下请求检索由对象 **ID** 标识的应用的 id 和 **requiredResourceAccess** **属性** `581088ba-83c5-4975-b8af-11d2d7a76e98` 。

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/applications/581088ba-83c5-4975-b8af-11d2d7a76e98?$select=id,requiredResourceAccess
```

>**注意：** 虽然你已配置应用所需的权限，但是尚未授予这些权限。 许多权限都需要获得管理员同意，然后才能用于访问组织数据。

## <a name="option-2-use-microsoft-graph-powershell"></a>选项 2：使用 Microsoft Graph PowerShell

Microsoft Graph PowerShell 中的 [Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true) cmdlet 包括 **RequiredResourceAccess** 参数，该参数是 **IMicrosoftGraphRequiredResourceAccess** 对象的集合。 使用此参数配置所需的Azure AD Graph权限，如以下步骤所述。

### <a name="prerequisites"></a>先决条件

若要完成以下步骤，需要以下权限：

+ 身份验证的 PowerShell 会话 (，例如，使用 `Connect-MgGraph`) 。
+ Microsoft Graph PowerShell 必须被授予 `Application.ReadWrite.All` 权限。
+ 登录用户必须被授予全局管理员或应用程序管理员Azure AD目录角色，或者成为目标应用注册的所有者。 有关这些角色支持的操作详细信息，请参阅Azure AD[角色](/azure/active-directory/roles/permissions-reference)。

### <a name="step-1-identify-the-permission-ids-for-the-azure-ad-graph-permissions-your-app-requires"></a>步骤 1：确定应用Azure AD Graph权限的权限标识

确定Azure AD Graph所需的权限、其权限标识，以及它们是应用程序角色 (应用程序权限) 委派权限。 可以通过在 Azure 门户上的应用清单中读取 **RequiredResourceAccess** 属性，或者通过 PowerShell 脚本，从具有配置权限的现有应用注册中检索权限 ID。

### <a name="request"></a>请求

创建一个名为fetchPermissions.ps1 **的新** PowerShell 脚本并添加以下代码。 此代码从Azure AD Graph ID 标识的现有应用注册中检索权限 ID 和类型 `f7748341-825c-46e9-a111-5e3b56ae015b` 。 将 `f7748341-825c-46e9-a111-5e3b56ae015b` 替换为源应用的对象 ID。

```powershell
# Sign in with the required Application.ReadWrite.All scope
Connect-Graph -Scopes "Application.ReadWrite.All" 

## Replace f7748341-825c-46e9-a111-5e3b56ae015b with the object ID of the existing app registration; then read and output the permission IDs and their types
$sourceAppId= 'f7748341-825c-46e9-a111-5e3b56ae015b' 
$sourceApp = Get-MgApplication -ApplicationId $sourceAppId 
$sourceApp.RequiredResourceAccess.ResourceAccess
```

运行以下命令的脚本
```powershell
.\fetchPermissions.ps1
```

### <a name="response"></a>响应

下面是一个输出示例。

```powershell
Id                                   Type
--                                   ----
311a71cc-e848-46a1-bdf8-97ff7156d8e6 Scope
3afa6a7d-9b1a-42eb-948e-1650a849e176 Role
```

在此输出中， `311a71cc-e848-46a1-bdf8-97ff7156d8e6` 是 *User.Read* 委派权限的权限 `3afa6a7d-9b1a-42eb-948e-1650a849e176` ID，而 是 *Application.Read.All* 应用程序角色的权限 ID。

### <a name="step-2-add-azure-ad-graph-permissions-to-your-app"></a>步骤 2：Azure AD Graph应用程序添加权限

创建一个名为updatePermissions.ps1 **的新** PowerShell 脚本并添加以下代码。 此代码将所需的Azure AD Graph添加到对象 ID 标识的应用注册 `581088ba-83c5-4975-b8af-11d2d7a76e98` 。 在步骤 1 中，这些权限分别为 *User.Read* 和 *Application.Read.All* 委派权限和应用程序角色。

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
