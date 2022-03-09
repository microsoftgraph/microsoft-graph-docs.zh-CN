---
title: 将应用程序权限限制为特定 Exchange Online 邮箱
description: 若要将应用程序权限界定为特定 Exchange Online 邮箱，你需要创建应用程序访问策略。
author: abheek-das
ms.localizationpriority: high
ms.prod: applications
ms.openlocfilehash: 03a0edde1a3e21455200049bf51bf1867e1a0657
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335890"
---
# <a name="limiting-application-permissions-to-specific-exchange-online-mailboxes"></a>将应用程序权限限制为特定 Exchange Online 邮箱 

想要限制对特定邮箱的应用访问权限的管理员可以使用 **New-ApplicationAccessPolicy** PowerShell cmdlet 创建应用程序访问策略。 本文介绍配置访问控制的基本步骤。 这些步骤仅适用于 Exchange Online 资源，不适用于其他 Microsoft Graph 工作负载。 

## <a name="background"></a>背景
一些应用使用他们自己的标识（而不代表用户）调用 Microsoft Graph。 这些是在服务器上运行的后台服务或守护程序，不存在登录用户。 这些应用使用 [OAuth 2.0 客户端凭据授予流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)进行身份验证，并使用应用程序权限进行配置，默认情况下，这些应用可以访问 exchange Online 上组织中的 _所有_ 邮箱。 例如， `Mail.Read` 应用程序权限允许应用在没有登录用户的情况下读取所有邮箱中的邮件。

> [!IMPORTANT]
> 
> 默认情况下，已将应用程序权限授予以下数据集的应用可访问组织中的所有邮箱：
> 
> - [日历](permissions-reference.md#calendars-permissions)
> - [联系人](permissions-reference.md#contacts-permissions)
> - [邮件](permissions-reference.md#mail-permissions)
> - [邮箱设置](permissions-reference.md#mail-permissions)
> 
>管理员可以配置 [应用程序访问策略](#configure-applicationaccesspolicy)，以限制对 _特定_ 邮箱的应用访问。

在某些情况下，管理员可能希望将应用限制为仅特定邮箱， _并非所有_ 组织中的 Exchange Online 邮箱。 管理员可以通过将邮箱放入启用邮件的安全组来标识允许访问的邮箱集。 然后，管理员可以通过创建用于访问该组的应用程序访问策略，将第三方应用访问权限限制为仅对该组的邮箱。

如以下 [支持的权限和其他资源](#supported-permissions-and-additional-resources) 部分中所述，应用程序访问策略限制已授予策略支持的任何Microsoft Graph或 Exchange Web 服务权限范围的应用的邮箱访问权限。

## <a name="configure-applicationaccesspolicy"></a>配置应用程序访问策略

若要配置应用程序访问策略并限制应用程序权限的范围：
1.  连接到 Exchange Online PowerShell。有关详细信息，请参见[连接到 Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)。

2.  标识应用客户端 ID 和限制应用可访问的启用邮件的安全组。

    - 在 [Azure 应用注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)中标识应用的应用程序（客户端）ID。
    - 创建新的启用邮件的安全组，或使用现有安全组并标识改组的电子邮件地址。 

3.  创建应用程序访问策略。 

    运行以下命令，替换 **AppId**、 **PolicyScopeGroupId** 和 **Description** 的参数。
    ```sh 
    New-ApplicationAccessPolicy -AppId e7e4dbfc-046f-4074-9b3b-2ae8f144f59b -PolicyScopeGroupId EvenUsers@contoso.com -AccessRight RestrictAccess -Description "Restrict this app to members of distribution group EvenUsers."
    ```
4.  测试新建的应用程序访问策略。

    运行以下命令，替换 **Identity** 的参数，并 **AppId**。
    ```sh
    Test-ApplicationAccessPolicy -Identity user1@contoso.com -AppId e7e4dbfc-046-4074-9b3b-2ae8f144f59b 
    ```
    此命令的输出将会指示该应用是否有权访问 User1 的邮箱。

>**注意：** 对应用程序访问策略的更改可能需要超过 1 小时才能在 Microsoft Graph REST API 调用中生效，即使 `Test-ApplicationAccessPolicy` 显示正面结果。

## <a name="supported-permissions-and-additional-resources"></a>受支持的权限和其他资源

管理员可以使用 ApplicationAccessPolicy cmdlet 来控制已授予以下任一Microsoft Graph应用程序权限或 Exchange Web 服务权限的应用的邮箱访问权限。 

Microsoft Graph应用程序权限： 
- `Mail.Read`
- `Mail.ReadBasic`
- `Mail.ReadBasic.All`
- `Mail.ReadWrite`
- `Mail.Send`
- `MailboxSettings.Read`
- `MailboxSettings.ReadWrite`
- `Calendars.Read`
- `Calendars.ReadWrite`
- `Contacts.Read`
- `Contacts.ReadWrite`

Exchange Web 服务权限范围： `full_access_as_app`。

有关配置应用程序访问策略的详细信息，请参阅[适合于 New-ApplicationAccessPolicy 的 PowerShell cmdlet 参考](/powershell/module/exchange/new-applicationaccesspolicy?view=exchange-ps&preserve-view=true)。 


## <a name="handling-api-errors"></a>处理 API 错误
当 API 调用访问因所配置的应用程序访问策略而遭拒时，你可能会遇到以下错误。 
```json
{
    "error": {
        "code": "ErrorAccessDenied",
        "message": "Access to OData is disabled.",
        "innerError": {
            "request-id": "2f038156-cf40-403d-8e46-831fe42a8229",
            "date": "2019-05-24T10:16:21"
        }
    }
}
```
如果应用Microsoft Graph API 调用返回此错误，请与组织的 Exchange Online 管理员协作，确保应用有权访问邮箱资源。



## <a name="see-also"></a>另请参阅

- [权限参考](permissions-reference.md)
- [New-ApplicationAccessPolicy](/powershell/module/exchange/organization/new-applicationaccesspolicy)
- [Get-ApplicationAccessPolicy](/powershell/module/exchange/organization/get-applicationaccesspolicy)
- [Remove-ApplicationAccessPolicy](/powershell/module/exchange/organization/remove-applicationaccesspolicy)
- [Set-ApplicationAccessPolicy](/powershell/module/exchange/organization/set-applicationaccesspolicy)
- [Test-ApplicationAccessPolicy](/powershell/module/exchange/organization/test-applicationaccesspolicy)
- [EWS 中的应用程序访问策略支持](https://techcommunity.microsoft.com/t5/exchange-team-blog/application-access-policy-support-in-ews/ba-p/2110361)
