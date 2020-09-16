---
title: 允许 applicatiosn 代表用户访问在线会议
description: 了解如何配置应用程序以代表用户访问在线会议。
author: frankpeng7
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 8f0738d282cfe012b90293b067c87ab7dc284f9e
ms.sourcegitcommit: 7e1993d64cc6d3145ae0ca984fefe74772b6052b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/16/2020
ms.locfileid: "47843341"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a>允许应用程序代表用户访问在线会议

在某些情况下，例如，对于在不存在登录用户的服务器上运行的后台服务或守护程序应用程序，应用程序可以调用 Microsoft Graph 以代表用户执行操作。 例如，应用可能需要调用 Microsoft Graph，以根据发布的日程安排多个会议 (例如课程) 或外部计划工具。 在这些情况下，应用程序代表的用户标识为会议组织者。

希望允许应用程序代表用户访问联机会议资源的管理员可以使用 **CsApplicationAccessPolicy** 和 **CsApplicationAccessPolicy** PowerShell cmdlet 配置访问控制。 本文介绍了配置应用程序访问策略的基本步骤。

这些步骤特定于联机会议，不应用于其他 Microsoft Graph 资源。

## <a name="configure-application-access-policy"></a>配置应用程序访问策略

若要配置应用程序访问策略并允许应用程序使用应用程序权限访问联机会议，请执行以下操作：

1. 标识应用程序的 applcation (客户端) ID 和代表用户的用户 Id，该应用程序将被授权访问联机会议。

    - 在 [Azure 应用注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)中标识应用的应用程序（客户端）ID。
    - 在[Azure 用户管理门户](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)中标识用户的用户 (对象) ID

2. 使用 adminitrator 帐户连接到 Skype for Business PowerShell。 有关详细信息，请参阅 [使用 PowerShell 管理 Skype For Business Online](https://docs.microsoft.com/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell)。

3. 创建包含应用程序 Id 列表的应用程序访问策略。

    运行以下 cmdlet，将 **Identity**、 **AppIds**和 **Description** 替换 (可选的) 参数。

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. 向用户授予策略，以便允许包含在策略中的应用程序 Id 代表授予用户访问联机会议。 

   运行以下 cmdlet 以替换 **PolicyName** 和 **Identity** 参数。

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> **注意** 
> 
> - _标识_ 是指创建策略时的策略名称，但在授予策略时是用户 ID。
> - 对应用程序访问策略所做的更改可能需要30分钟才能在 Microsoft Graph REST API 调用中生效。

## <a name="supported-permissions-and-additional-resources"></a>受支持的权限和其他资源

管理员可以使用 ApplicationAccessPolicy cmdlet 来控制已授予以下任一应用程序权限的应用的邮箱访问权限：

- OnlineMeetings.Read.All
- OnlineMeetings.ReadWrite.All

有关配置应用程序访问策略的详细信息，请参阅[适合于 New-ApplicationAccessPolicy 的 PowerShell cmdlet 参考](https://docs.microsoft.com/powershell/module/skype/new-csapplicationaccesspolicy)。

## <a name="errors"></a>错误

如果在未配置应用程序访问策略时试图访问联机会议的应用程序导致 API 调用被拒绝，则可能会遇到以下错误。

```json
{
    "error": {
        "code": "Unauthorized",
        "message": "App <app_ID_redacted> is not authorized to Create meeting on behalf of user <user_ID_redacted>",
        "innerError": {
            "date": "<date_redacted>",
            "request-id": "599d9cb0-56ac-4dc5-b6f8-1456a1414609"
        }
    }
}
```

按照本文中的步骤操作，创建和/或将包含应用程序 ID 的应用程序访问策略授予用户 ID。

## <a name="see-also"></a>另请参阅

- [权限参考](permissions-reference.md)
- [New-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/skype/new-csapplicationaccesspolicy)
- [Grant-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/skype/grant-csapplicationaccesspolicy)
- [Get-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/skype/get-csapplicationaccesspolicy)
- [Set-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/skype/set-csapplicationaccesspolicy)
- [Remove-ApplicationAccessPolicy](https://docs.microsoft.com/powershell/module/skype/remove-csapplicationaccesspolicy)
