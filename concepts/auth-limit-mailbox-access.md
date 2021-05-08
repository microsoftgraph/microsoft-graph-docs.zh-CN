---
title: 将应用程序权限界定为特定 Exchange Online 邮箱
description: 若要将应用程序权限界定为特定 Exchange Online 邮箱，你需要创建应用程序访问策略。
author: abheek-das
localization_priority: Priority
ms.prod: applications
ms.openlocfilehash: f31f7bfc8ff72c8f3cb9e6f61185187f50bab7fc
ms.sourcegitcommit: de3bc91a24d23b46bd0863487415fba8d8fce63c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/07/2021
ms.locfileid: "52266834"
---
# <a name="scoping-application-permissions-to-specific-exchange-online-mailboxes"></a>将应用程序权限界定为特定 Exchange Online 邮箱 

一些应用使用他们自己的标识（而不代表用户）调用 Microsoft Graph。 这些是在服务器上运行的后台服务或守护程序，不存在登录用户。 这些应用使用 [OAuth 2.0 客户端凭据授权流](/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)来进行身份验证并配置应用程序权限，这使得这些应用能够访问组织在 Exchange Online 上的所有邮箱。 例如，Mail.Read 应用程序权限使应用能够读取所有邮箱中的邮件而无需用户登录。 

管理员如果想要将应用限制为访问特定邮箱集，则可以使用 **New-ApplicationAccessPolicy** PowerShell cmdlet 来配置访问权限。 本文介绍了配置应用程序访问策略的基本步骤。

这些步骤仅适用于 Exchange Online 资源，不适用于其他 Microsoft Graph 工作负载。 

## <a name="configure-applicationaccesspolicy"></a>配置应用程序访问策略

若要配置应用程序访问策略并限制应用程序权限的范围：
1.  连接到 Exchange Online PowerShell。有关详细信息，请参见[连接到 Exchange Online PowerShell](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)。

2.  标识应用客户端 ID 和限制应用可访问的启用邮件的安全组。

    - 在 [Azure 应用注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)中标识应用的应用程序（客户端）ID。
    - 创建新的启用邮件的安全组，或使用现有安全组并标识改组的电子邮件地址。 

3.  创建应用程序访问策略。 

    运行以下命令，以替换 **AppId**、**PolicyScopeGroupId** 和 **Description** 参数。
    ```sh 
    New-ApplicationAccessPolicy -AppId e7e4dbfc-046f-4074-9b3b-2ae8f144f59b -PolicyScopeGroupId EvenUsers@contoso.com -AccessRight RestrictAccess -Description "Restrict this app to members of distribution group EvenUsers."
    ```
4.  测试新建的应用程序访问策略。

    运行以下命令，以替换 **AppId** 和 **Identity** 参数。
    ```sh
    Test-ApplicationAccessPolicy -Identity user1@contoso.com -AppId e7e4dbfc-046-4074-9b3b-2ae8f144f59b 
    ```
    此命令的输出将会指示该应用是否有权访问 User1 的邮箱。

>**注意：在 Microsoft Graph REST API 调用中，应用程序访问策略变更需要 30 分钟才能生效。**

## <a name="supported-permissions-and-additional-resources"></a>受支持的权限和其他资源
管理员可以使用 ApplicationAccessPolicy cmdlet 来控制已授权以下任何应用程序权限的应用的邮箱访问权限： 
- Mail.Read
- Mail.ReadBasic
- Mail.ReadBasic.All
- Mail.ReadWrite
- Mail.Send
- MailboxSettings.Read  
- MailboxSettings.ReadWrite
- Calendars.Read
- Calendars.ReadWrite
- Contacts.Read
- Contacts.ReadWrite

有关配置应用程序访问策略的详细信息，请参阅[适合于 New-ApplicationAccessPolicy 的 PowerShell cmdlet 参考](/powershell/module/exchange/organization/new-applicationaccesspolicy)。 

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
如果应用的 Microsoft Graph API 调用返回此错误，请与组织的 Exchange Online 管理员协作，确保你的应用具有邮箱资源的访问权限。



## <a name="see-also"></a>另请参阅

- [权限参考](permissions-reference.md)
- [New-ApplicationAccessPolicy](/powershell/module/exchange/organization/new-applicationaccesspolicy)
- [Get-ApplicationAccessPolicy](/powershell/module/exchange/organization/get-applicationaccesspolicy)
- [Remove-ApplicationAccessPolicy](/powershell/module/exchange/organization/remove-applicationaccesspolicy)
- [Set-ApplicationAccessPolicy](/powershell/module/exchange/organization/set-applicationaccesspolicy)
- [Test-ApplicationAccessPolicy](/powershell/module/exchange/organization/test-applicationaccesspolicy)
