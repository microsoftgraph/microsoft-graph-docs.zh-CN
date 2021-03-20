---
title: 允许应用程序代表用户访问联机会议
description: 了解如何配置应用程序以代表用户访问联机会议。
author: jsandoval-msft
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 23f46fec732895d33b2caa08c51493e9b5999b29
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961837"
---
# <a name="allow-applications-to-access-online-meetings-on-behalf-of-a-user"></a>允许应用程序代表用户访问联机会议

在某些情况下，例如对于在服务器上运行的后台服务或守护程序应用，在没有登录用户的情况下运行，应用可以代表用户调用 Microsoft Graph 来采取措施。 例如，应用可能需要调用 Microsoft Graph，根据已发布的计划安排多个会议， (课程) 外部计划工具。 在这些情况下，应用程序代表的用户将被标识为会议组织者。

希望允许应用程序代表用户访问联机会议资源的管理员可以使用 **New-CsApplicationAccessPolicy** 和 **Grant-CsApplicationAccessPolicy** PowerShell cmdlet 配置访问控制。 本文介绍了配置应用程序访问策略的基本步骤。

这些步骤特定于联机会议，不适用于其他 Microsoft Graph 资源。

## <a name="configure-application-access-policy"></a>配置应用程序访问策略

要配置应用程序访问策略并允许应用程序访问具有应用程序权限的联机会议，请执行：

1. 确定应用的应用 (客户端) ID 以及将授权应用访问联机会议的用户的用户 ID。

    - 在 [Azure 应用注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)中标识应用的应用程序（客户端）ID。
    - 在 Azure 用户管理门户 (用户) 标识 [用户对象 ID](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)

2. 使用管理员帐户连接到 Skype for Business PowerShell。 有关详细信息，请参阅使用 PowerShell 管理[Skype for Business Online。](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell)

3. 创建包含应用 ID 列表的应用程序访问策略。

    运行以下 cmdlet，将Identity、AppIds 和 **Description** (可选) 参数。 

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. 向用户授予策略，以允许策略中包含的应用 ID 代表已授予用户访问联机会议。 

   运行以下 cmdlet，替换 **PolicyName 和** **Identity** 参数。

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "ddb80e06-92f3-4978-bc22-a0eee85e6a9e"
   ```

> **注意** 
> 
> - _Identity_ 指创建策略时的策略名称，但在授予策略时指用户 ID。
> - 对应用程序访问策略的更改最多可能需要 30 分钟才能在 Microsoft Graph REST API 调用中生效。

## <a name="supported-permissions-and-additional-resources"></a>受支持的权限和其他资源

管理员可以使用 ApplicationAccessPolicy cmdlet 控制已被授予以下任一应用程序权限的应用的邮箱访问权限：

- OnlineMeetings.Read.All
- OnlineMeetings.ReadWrite.All

有关配置应用程序访问策略的详细信息，请参阅[适合于 New-ApplicationAccessPolicy 的 PowerShell cmdlet 参考](/powershell/module/skype/new-csapplicationaccesspolicy)。

## <a name="errors"></a>错误

当 API 调用因应用在未配置应用程序访问策略时尝试访问联机会议而被拒绝访问时，可能会遇到以下错误。

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

按照本文中的步骤创建和/或向用户 ID 授予包含应用 ID 的应用程序访问策略。

## <a name="see-also"></a>另请参阅

- [权限参考](permissions-reference.md)
- [New-CsApplicationAccessPolicy](/powershell/module/skype/new-csapplicationaccesspolicy)
- [Grant-CsApplicationAccessPolicy](/powershell/module/skype/grant-csapplicationaccesspolicy)
- [Get-CsApplicationAccessPolicy](/powershell/module/skype/get-csapplicationaccesspolicy)
- [Set-CsApplicationAccessPolicy](/powershell/module/skype/set-csapplicationaccesspolicy)
- [Remove-CsApplicationAccessPolicy](/powershell/module/skype/remove-csapplicationaccesspolicy)
