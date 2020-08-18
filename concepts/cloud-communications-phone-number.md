---
title: 管理机器人的电话号码
description: 本文介绍如何创建可通过电话号码访问的机器人。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 2dc201ff9423b0190daa5adf86871972cc577304
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792868"
---
# <a name="manage-phone-numbers-for-bots"></a>管理机器人的电话号码 

本文介绍如何创建可通过电话号码访问的机器人。 在创建你的 bot 时，熟悉以下术语将很有帮助：

- **应用程序** –托管在 Azure 上的应用程序（也称为 **bot**）。

- **应用程序实例** –可分配给机器人可使用的电话号码的已禁用用户对象。 这也称为 [资源帐户](https://docs.microsoft.com/microsoftteams/manage-resource-accounts)。 这是可以将电话号码分配给 bot 的唯一方法。

一个应用程序可以有多个应用程序实例，每个租户可以有多个应用程序实例，如下图所示。

![显示具有一个或多个应用程序实例的租户的电话号码的图像](images/communications-app-tenant.PNG)

## <a name="prerequisite---register-a-bot"></a>先决条件-注册 bot
若要开始，请按照说明 [注册呼叫机器人](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html)。 你将需要在代码中使用的配置值（如 bot ID、Microsoft app ID 和 Microsoft 应用密码）。

向你的 bot 添加以下权限。 租户管理员还需要同意这些权限：

- Calls.AccessMedia.All
- Calls.Initiate.All
- Calls.JoinGroupCall.All
- JoinGroupCallAsGuest

有关与呼叫相关的权限的详细信息，请参阅 [权限参考](permissions-reference.md#calls-permissions)。


## <a name="assign-a-phone-number-to-your-bot"></a>将电话号码分配给你的机器人

为你的 bot 分配电话号码包括三个步骤：

1.  创建应用程序实例。
2.  将虚拟用户许可证分配给应用程序实例。
3.  仅 (租户管理员) 向应用程序实例分配电话号码。

### <a name="create-an-application-instance"></a>创建应用程序实例

如果尚未安装，租户管理员需要为 PowerShell 安装 [Skype For Business Online 模块](https://www.microsoft.com/download/details.aspx?id=39366) 。 租户管理员必须先使用其凭据登录，然后才能运行 cmdlet。

若要创建新的应用程序实例，租户管理员需要运行以下 cmdlet。

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId “<app_id>” -DisplayName "<bot_display_name>"`

创建应用程序实例时，请使用 sync cmdlet。

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

### <a name="assign-a-virtual-user-license-to-your-application-instance"></a>将虚拟用户许可证分配给应用程序实例

将虚拟用户许可证分配给应用程序实例。 有关详细信息，请参阅 [电话系统虚拟用户许可证](https://docs.microsoft.com/microsoftteams/teams-add-on-licensing/virtual-user)。

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a>仅将电话号码分配给应用程序实例 (仅租户管理员) 

若要将电话号码分配给应用程序实例，租户管理员请执行以下操作：

1. 以租户管理员身份登录到团队管理中心。
2. 转到 "**团队管理员中心**"  >  **语音**  >  **电话号码**。
3. 使用以下 cmdlet 将服务电话号码分配 (+ 11D 格式) 。

  `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`

## <a name="unassign-a-bot-phone-number"></a>取消分配机器人电话号码

使用以下 cmdlet 取消分配电话号码。

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

>**注意：** 目前，这仅适用于联机号码，而不是直接路由 (DR) 号码。 这是一个已知问题。

## <a name="update-a-bot-phone-number"></a>更新机器人电话号码

取消分配号码后，可以使用以下 cmdlet 为 bot 分配其他号码。

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a>另请参阅

- [事件 bot 示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot)。 
 - 有关如何部署的详细信息，请参阅 [部署示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample)。

