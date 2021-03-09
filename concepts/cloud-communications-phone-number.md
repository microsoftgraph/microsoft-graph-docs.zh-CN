---
title: 管理机器人的电话号码
description: 本文介绍如何创建可以通过电话号码访问的自动程序。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: d6b71d2db1be951137ca33026f243dae6055c93f
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50573570"
---
# <a name="manage-phone-numbers-for-bots"></a>管理机器人的电话号码 

本文介绍如何创建可以通过电话号码访问的自动程序。 创建自动程序时，熟悉以下术语会很有帮助：

- **应用程序** – 托管在 Azure 上的应用程序，也称为自动 **程序**。

- **应用程序** 实例 – 可分配给机器人可以使用的电话号码的已禁用用户对象。 这也称为资源 [帐户](/microsoftteams/manage-resource-accounts)。 这是将电话号码分配给自动程序的唯一方式。

一个应用程序可以有多个应用程序实例，每个租户可以有多个应用程序实例，如下图所示。

![显示具有一个或多个应用程序实例的租户的电话号码的图像](images/communications-app-tenant.PNG)

## <a name="prerequisite---register-a-bot"></a>先决条件 - 注册自动程序
若要开始，请按照说明 [注册呼叫机器人](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html)。 你需要配置值，如自动程序 ID、Microsoft 应用 ID 和 Microsoft 应用密码，才能在代码中使用。

将以下权限添加到自动程序。 租户管理员还需要同意这些权限：

- Calls.AccessMedia.All
- Calls.Initiate.All
- Calls.JoinGroupCall.All
- Calls.JoinGroupCallAsGuest.All

有关与呼叫相关的权限详细信息，请参阅 ["权限"参考](permissions-reference.md#calls-permissions)。


## <a name="assign-a-phone-number-to-your-bot"></a>将电话号码分配给机器人

将电话号码分配给自动程序涉及三个步骤：

1.  创建应用程序实例。
2.  将 Microsoft 365 许可证分配给应用程序实例。
3.  将电话号码分配给应用程序实例 (租户管理员) 。

### <a name="create-an-application-instance"></a>创建应用程序实例

如果尚未安装，租户管理员需要安装适用于 PowerShell 的 [Skype for Business Online](https://www.microsoft.com/download/details.aspx?id=39366) 模块。 租户管理员必须在运行 cmdlet 之前使用其凭据登录。

若要创建新的应用程序实例，租户管理员将运行以下 cmdlet。

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId <app_id> -DisplayName <bot_display_name>`

创建应用程序实例时，请使用同步 cmdlet。

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

有关详细信息，请参阅 [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。

### <a name="assign-microsoft-365-licenses-to-your-application-instance"></a>将 Microsoft 365 许可证分配给应用程序实例

向应用程序实例分配虚拟用户许可证。 有关详细信息，请参阅 [电话系统虚拟用户许可证](/microsoftteams/teams-add-on-licensing/virtual-user)。

将通话套餐分配给应用程序实例。 有关详细信息，请参阅 [Microsoft 365](/microsoftteams/calling-plans-for-office-365)的通话套餐。

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a>将电话号码分配给应用程序实例 (仅租户管理员) 

在可以将组织中的用户设置为拨打和接听电话前，必须为其获取电话号码。 有关详细信息，请参阅 [获取用户的电话号码](/microsoftteams/getting-phone-numbers-for-your-users#get-new-phone-numbers-for-your-users)。

若要将电话号码分配给应用程序实例，租户管理员：

1. 以租户管理员登录 Teams 管理中心。
2. 转到 **Teams 管理中心**  >  **语音**  >  **电话号码**。
3. 使用以下 cmdlet (+11D 格式) 服务电话号码。

  `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`
  
分配服务电话号码时，请使用同步 cmdlet。

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

有关详细信息，请参阅 [Set-CsOnlineVoiceApplicationInstance](/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。

## <a name="unassign-a-bot-phone-number"></a>取消分配自动程序电话号码

使用以下 cmdlet 取消分配电话号码。

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

>**注意：** 目前，这仅适用于联机号码，不能直接路由 (DR) 号码。 这是一个已知问题。

## <a name="update-a-bot-phone-number"></a>更新自动程序电话号码

取消分配号码后，可以通过以下 cmdlet 为自动程序分配不同的号码。

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a>另请参阅

- [事件机器人示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot)。 
 - 若要详细了解如何部署，请参阅 [部署示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample)。
