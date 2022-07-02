---
title: 使用云通信 API 配置应用程序访问策略
description: 使用 Microsoft Graph 中的云通信 API 配置访问策略，允许应用程序代表用户访问联机会议。
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 89015fffb8713f00f7d54d9eaa8e43272d03ca45
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436352"
---
# <a name="configure-application-access-to-online-meetings"></a>配置对联机会议的应用程序访问权限

可以使用 Microsoft Graph 中的云通信 API 配置应用程序访问策略，允许应用程序代表用户访问联机会议。

在某些情况下，例如，对于在没有登录用户的情况下在服务器上运行的后台服务或守护程序应用，应用应代表用户调用 Microsoft Graph 以执行操作。 例如，应用可能需要调用 Microsoft Graph，以便根据已发布的计划 (（例如课程) 或外部计划工具）安排多个会议。 在这些情况下，应用程序代表的用户被标识为会议组织者。

希望允许应用程序代表用户访问联机会议资源的管理员可以使用 **New-CsApplicationAccessPolicy** 和 **Grant-CsApplicationAccessPolicy** PowerShell cmdlet 来配置访问控制。

本文介绍了配置应用程序访问策略的基本步骤。 这些步骤特定于联机会议，不适用于其他 Microsoft Graph 资源。

## <a name="configure-application-access-policy"></a>配置应用程序访问策略

若要配置应用程序访问策略并允许应用程序使用应用程序权限访问联机会议，请执行以下操作：

1. 标识应用的应用程序 (客户端) ID 和用户的用户 ID，代表这些用户，应用将有权访问联机会议。

    - 在 [Azure 应用注册门户](https://portal.azure.com/#blade/Microsoft_AAD_RegisteredApps/ApplicationsListBlade)中标识应用的应用程序（客户端）ID。
    - 在 [Azure 用户管理门户](https://portal.azure.com/#blade/Microsoft_AAD_IAM/UsersManagementMenuBlade)中标识用户的用户 (对象) ID

2. 使用管理员帐户连接到 Skype for Business PowerShell。 有关详细信息，请参阅[使用 PowerShell 管理 Skype for Business Online](/microsoft-365/enterprise/manage-skype-for-business-online-with-microsoft-365-powershell)。

3. 创建包含应用 ID 列表的应用程序访问策略。

    运行以下 cmdlet，替换 **标识**、 **AppId 和** **Description** (可选) 参数。

    ```powershell
    New-CsApplicationAccessPolicy -Identity Test-policy -AppIds "ddb80e06-92f3-4978-bc22-a0eee85e6a9e", "ccb80e06-92f3-4978-bc22-a0eee85e6a9e", "bbb80e06-92f3-4978-bc22-a0eee85e6a9e" -Description "description here"
    ```

4. 向用户授予策略，以允许策略中包含的应用 ID 代表授予的用户访问联机会议。 

   运行以下 cmdlet，替换 **PolicyName** 和 **Identity** 参数。

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Identity "748d2cbb-3b55-40ed-8c34-2eae5932b22a"
   ```
5.  (可选) 向整个租户授予策略。 这适用于未分配应用程序访问策略的用户。 有关详细信息，请参阅另 [请参阅](#see-also) 部分中的 cmdlet 链接。

   运行以下 cmdlet，替换 **PolicyName** 参数。

   ```powershell
   Grant-CsApplicationAccessPolicy -PolicyName Test-policy -Global
   ```

> [!NOTE]
> - _标识_ 在创建策略时引用策略名称，但在授予策略时指用户 ID。
> - 对应用程序访问策略的更改可能需要长达 30 分钟才能在 Microsoft Graph REST API 调用中生效。

## <a name="supported-permissions-and-additional-resources"></a>受支持的权限和其他资源

管理员可以使用 ApplicationAccessPolicy cmdlet 控制已被授予以下任何应用程序权限的应用的联机会议访问：

- OnlineMeetings.Read.All
- OnlineMeetings.ReadWrite.All
- OnlineMeetingArtifact.Read.All

有关配置应用程序访问策略的详细信息，请参阅[适合于 New-ApplicationAccessPolicy 的 PowerShell cmdlet 参考](/powershell/module/skype/new-csapplicationaccesspolicy)。

## <a name="errors"></a>错误

当未配置应用程序访问策略时，由于应用尝试访问联机会议，API 调用被拒绝访问时，可能会遇到以下错误。

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
- [云通信 API 概述](cloud-communications-concept-overview.md)
