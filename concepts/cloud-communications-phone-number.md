---
title: 使用云通信 API 管理机器人的电话号码
description: 了解如何使用 Microsoft Graph 云通信 API 创建可通过电话号码访问的机器人，以及如何分配、取消分配或更新机器人电话号码。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
ms.openlocfilehash: 607fbcb9dd522364ba3e5ec69e80ac2d93ddfe8b
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66440962"
---
# <a name="manage-phone-numbers-for-bots"></a>管理机器人的电话号码

本文介绍如何使用 Microsoft Graph 中的云通信 API 创建可通过电话号码访问的机器人。 创建机器人时，熟悉以下术语会很有帮助：

- **应用：** 托管在 Azure 上的应用程序，也称为 **机器人**。

- **应用程序实例：** 可分配给机器人可以使用的电话号码的禁用用户对象。 这也称为 [资源帐户](/microsoftteams/manage-resource-accounts)。 这是将电话号码分配给机器人的唯一方法。

一个应用程序可以有多个应用程序实例，每个租户可以有多个应用程序实例，如下图所示。

![显示具有一个或多个应用程序实例的租户的电话号码的图像](images/communications-app-tenant.PNG)

## <a name="prerequisite-register-a-bot"></a>先决条件：注册机器人

若要开始，请按照说明 [注册调用机器人](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html)。 需要在代码中使用机器人 ID、Microsoft 应用 ID 和 Microsoft 应用密码等配置值。

将以下权限添加到机器人。 租户管理员也需要同意这些权限：

- Calls.AccessMedia.All
- Calls.Initiate.All
- Calls.JoinGroupCall.All
- Calls.JoinGroupCallAsGuest.All

有关与呼叫相关的权限的详细信息，请参阅 [“权限”参考](permissions-reference.md#calls-permissions)。

## <a name="assign-a-phone-number-to-your-bot"></a>将电话号码分配给机器人

向机器人分配电话号码涉及三个步骤：

1. 创建应用程序实例。
2. 将 Microsoft 365 许可证分配到应用程序实例。
3. 将电话号码分配给应用程序实例 (仅租户管理员) 。

### <a name="create-an-application-instance"></a>创建应用程序实例

如果尚未安装，租户管理员需要安装 [Skype for Business Online Module](https://www.microsoft.com/download/details.aspx?id=39366) for PowerShell。 租户管理员在运行 cmdlet 之前必须使用其凭据登录。

若要创建新的应用程序实例，租户管理员运行以下 cmdlet：

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId <app_id> -DisplayName <bot_display_name>`

创建应用程序实例时，请使用同步 cmdlet：

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

有关详细信息，请参阅 [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。

### <a name="assign-microsoft-365-licenses-to-your-application-instance"></a>将 Microsoft 365 许可证分配到应用程序实例

将虚拟用户许可证分配到应用程序实例。 有关详细信息，请参阅 [电话系统虚拟用户许可证](/microsoftteams/teams-add-on-licensing/virtual-user)。

将调用计划分配给应用程序实例。 有关详细信息，请参阅 [Microsoft 365 的呼叫计划](/microsoftteams/calling-plans-for-office-365)。

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a>将电话号码分配给应用程序实例 (仅租户管理员) 

在进行组织用户拨打和接听电话的设置之前，必须先为用户获取电话号码。 有关详细信息，请参阅 [获取用户的电话号码](/microsoftteams/getting-phone-numbers-for-your-users#get-new-phone-numbers-for-your-users)。

要将电话号码分配到应用程序实例，租户管理员：

1. 以租户管理员身份登录到 Teams 管理中心。
2. 转到 **Teams 管理员中心** > **语音** > **电话号码**。
3. 使用以下 cmdlet) 分配服务电话号码 (+11D 格式：

   `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`
  
分配服务电话号码时，请使用同步 cmdlet：

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

有关详细信息，请参阅 [Set-CsOnlineVoiceApplicationInstance](/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。

## <a name="unassign-a-bot-phone-number"></a>取消分配机器人电话号码

使用以下 cmdlet 取消分配电话号码：

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

> [!NOTE]
> 目前，这仅适用于联机数字，而不适用于直接路由 (DR) 数字。 这是一个已知问题。

## <a name="update-a-bot-phone-number"></a>更新机器人电话号码

取消分配数字后，可以使用以下 cmdlet 将其他数字分配给机器人：

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a>另请参阅

- [云通信 API 概述](cloud-communications-concept-overview.md)
- [事件机器人示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/V1.0Samples/RemoteMediaSamples/IncidentBot)
- [部署示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/V1.0Samples/RemoteMediaSamples/README.md#deploying-the-sample)
