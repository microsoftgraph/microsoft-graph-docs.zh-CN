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
# <a name="manage-phone-numbers-for-bots"></a><span data-ttu-id="5d9b0-103">管理机器人的电话号码</span><span class="sxs-lookup"><span data-stu-id="5d9b0-103">Manage phone numbers for bots</span></span> 

<span data-ttu-id="5d9b0-104">本文介绍如何创建可以通过电话号码访问的自动程序。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-104">This article describes how to create a bot that is reachable through a phone number.</span></span> <span data-ttu-id="5d9b0-105">创建自动程序时，熟悉以下术语会很有帮助：</span><span class="sxs-lookup"><span data-stu-id="5d9b0-105">As you create your bot, it will be helpful to be familiar with the following terms:</span></span>

- <span data-ttu-id="5d9b0-106">**应用程序** – 托管在 Azure 上的应用程序，也称为自动 **程序**。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-106">**Application** – An application that is hosted on Azure, also referred to as a **bot**.</span></span>

- <span data-ttu-id="5d9b0-107">**应用程序** 实例 – 可分配给机器人可以使用的电话号码的已禁用用户对象。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-107">**Application instance** – A disabled-user object that can be assigned to a phone number that can be used by a bot.</span></span> <span data-ttu-id="5d9b0-108">这也称为资源 [帐户](/microsoftteams/manage-resource-accounts)。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-108">This is also known as a [resource account](/microsoftteams/manage-resource-accounts).</span></span> <span data-ttu-id="5d9b0-109">这是将电话号码分配给自动程序的唯一方式。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-109">This is the only way a phone number can be assigned to a bot.</span></span>

<span data-ttu-id="5d9b0-110">一个应用程序可以有多个应用程序实例，每个租户可以有多个应用程序实例，如下图所示。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-110">One application can have multiple application instances, and each tenant can have multiple application instances, as shown in the following image.</span></span>

![显示具有一个或多个应用程序实例的租户的电话号码的图像](images/communications-app-tenant.PNG)

## <a name="prerequisite---register-a-bot"></a><span data-ttu-id="5d9b0-112">先决条件 - 注册自动程序</span><span class="sxs-lookup"><span data-stu-id="5d9b0-112">Prerequisite - Register a bot</span></span>
<span data-ttu-id="5d9b0-113">若要开始，请按照说明 [注册呼叫机器人](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html)。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-113">To get started, follow the instructions to [register a calling bot](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html).</span></span> <span data-ttu-id="5d9b0-114">你需要配置值，如自动程序 ID、Microsoft 应用 ID 和 Microsoft 应用密码，才能在代码中使用。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-114">You’ll need config values such as bot ID, Microsoft app ID, and Microsoft app password to use in your code.</span></span>

<span data-ttu-id="5d9b0-115">将以下权限添加到自动程序。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-115">Add the following permissions to your bot.</span></span> <span data-ttu-id="5d9b0-116">租户管理员还需要同意这些权限：</span><span class="sxs-lookup"><span data-stu-id="5d9b0-116">A tenant admin needs to consent to these permissions as well:</span></span>

- <span data-ttu-id="5d9b0-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="5d9b0-117">Calls.AccessMedia.All</span></span>
- <span data-ttu-id="5d9b0-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="5d9b0-118">Calls.Initiate.All</span></span>
- <span data-ttu-id="5d9b0-119">Calls.JoinGroupCall.All</span><span class="sxs-lookup"><span data-stu-id="5d9b0-119">Calls.JoinGroupCall.All</span></span>
- <span data-ttu-id="5d9b0-120">Calls.JoinGroupCallAsGuest.All</span><span class="sxs-lookup"><span data-stu-id="5d9b0-120">Calls.JoinGroupCallAsGuest.All</span></span>

<span data-ttu-id="5d9b0-121">有关与呼叫相关的权限详细信息，请参阅 ["权限"参考](permissions-reference.md#calls-permissions)。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-121">For more information about call-related permissions, see the [Permissions reference](permissions-reference.md#calls-permissions).</span></span>


## <a name="assign-a-phone-number-to-your-bot"></a><span data-ttu-id="5d9b0-122">将电话号码分配给机器人</span><span class="sxs-lookup"><span data-stu-id="5d9b0-122">Assign a phone number to your bot</span></span>

<span data-ttu-id="5d9b0-123">将电话号码分配给自动程序涉及三个步骤：</span><span class="sxs-lookup"><span data-stu-id="5d9b0-123">Assigning a phone number to your bot involves three steps:</span></span>

1.  <span data-ttu-id="5d9b0-124">创建应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-124">Create an application instance.</span></span>
2.  <span data-ttu-id="5d9b0-125">将 Microsoft 365 许可证分配给应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-125">Assign Microsoft 365 licenses to your application instance.</span></span>
3.  <span data-ttu-id="5d9b0-126">将电话号码分配给应用程序实例 (租户管理员) 。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-126">Assign a phone number to the application instance (only tenant admin).</span></span>

### <a name="create-an-application-instance"></a><span data-ttu-id="5d9b0-127">创建应用程序实例</span><span class="sxs-lookup"><span data-stu-id="5d9b0-127">Create an application instance</span></span>

<span data-ttu-id="5d9b0-128">如果尚未安装，租户管理员需要安装适用于 PowerShell 的 [Skype for Business Online](https://www.microsoft.com/download/details.aspx?id=39366) 模块。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-128">If it hasn't been installed already, a tenant admin needs to install the [Skype for Business Online Module](https://www.microsoft.com/download/details.aspx?id=39366) for PowerShell.</span></span> <span data-ttu-id="5d9b0-129">租户管理员必须在运行 cmdlet 之前使用其凭据登录。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-129">The tenant admin must sign in using their credentials before running the cmdlet.</span></span>

<span data-ttu-id="5d9b0-130">若要创建新的应用程序实例，租户管理员将运行以下 cmdlet。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-130">To create a new application instance, the tenant admin runs the following cmdlet.</span></span>

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId <app_id> -DisplayName <bot_display_name>`

<span data-ttu-id="5d9b0-131">创建应用程序实例时，请使用同步 cmdlet。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-131">When the application instance is created, use the sync cmdlet.</span></span>

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

<span data-ttu-id="5d9b0-132">有关详细信息，请参阅 [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-132">For more information, see [New-CsOnlineApplicationInstance](/powershell/module/skype/new-csonlineapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>

### <a name="assign-microsoft-365-licenses-to-your-application-instance"></a><span data-ttu-id="5d9b0-133">将 Microsoft 365 许可证分配给应用程序实例</span><span class="sxs-lookup"><span data-stu-id="5d9b0-133">Assign Microsoft 365 licenses to your application instance</span></span>

<span data-ttu-id="5d9b0-134">向应用程序实例分配虚拟用户许可证。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-134">Assign a virtual user license to your application instance.</span></span> <span data-ttu-id="5d9b0-135">有关详细信息，请参阅 [电话系统虚拟用户许可证](/microsoftteams/teams-add-on-licensing/virtual-user)。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-135">For details, see [Phone system virtual user license](/microsoftteams/teams-add-on-licensing/virtual-user).</span></span>

<span data-ttu-id="5d9b0-136">将通话套餐分配给应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-136">Assign a calling plan to your application instance.</span></span> <span data-ttu-id="5d9b0-137">有关详细信息，请参阅 [Microsoft 365](/microsoftteams/calling-plans-for-office-365)的通话套餐。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-137">For details, see [Calling plans for Microsoft 365](/microsoftteams/calling-plans-for-office-365).</span></span>

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a><span data-ttu-id="5d9b0-138">将电话号码分配给应用程序实例 (仅租户管理员) </span><span class="sxs-lookup"><span data-stu-id="5d9b0-138">Assign a phone number to the application instance (only tenant admin)</span></span>

<span data-ttu-id="5d9b0-139">在可以将组织中的用户设置为拨打和接听电话前，必须为其获取电话号码。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-139">Before you can set up users in your organization to make and receive phone calls, you must get phone numbers for them.</span></span> <span data-ttu-id="5d9b0-140">有关详细信息，请参阅 [获取用户的电话号码](/microsoftteams/getting-phone-numbers-for-your-users#get-new-phone-numbers-for-your-users)。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-140">For details, see [Getting phone numbers for your users](/microsoftteams/getting-phone-numbers-for-your-users#get-new-phone-numbers-for-your-users).</span></span>

<span data-ttu-id="5d9b0-141">若要将电话号码分配给应用程序实例，租户管理员：</span><span class="sxs-lookup"><span data-stu-id="5d9b0-141">To assign the phone number to the application instance, the tenant admin:</span></span>

1. <span data-ttu-id="5d9b0-142">以租户管理员登录 Teams 管理中心。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-142">Signs in to the Teams admin center as a tenant admin.</span></span>
2. <span data-ttu-id="5d9b0-143">转到 **Teams 管理中心**  >  **语音**  >  **电话号码**。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-143">Goes to **Teams Admin center** > **Voice** > **Phone Numbers**.</span></span>
3. <span data-ttu-id="5d9b0-144">使用以下 cmdlet (+11D 格式) 服务电话号码。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-144">Assigns a service phone number (+11D format) using the following cmdlet.</span></span>

  `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`
  
<span data-ttu-id="5d9b0-145">分配服务电话号码时，请使用同步 cmdlet。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-145">When the service phone number is assigned, use the sync cmdlet.</span></span>

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

<span data-ttu-id="5d9b0-146">有关详细信息，请参阅 [Set-CsOnlineVoiceApplicationInstance](/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) 和 [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true)。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-146">For more information, see [Set-CsOnlineVoiceApplicationInstance](/powershell/module/skype/set-csonlinevoiceapplicationinstance?view=skype-ps&preserve-view=true) and [Sync-CsOnlineApplicationInstance](/powershell/module/skype/sync-csonlineapplicationinstance?view=skype-ps&preserve-view=true).</span></span>

## <a name="unassign-a-bot-phone-number"></a><span data-ttu-id="5d9b0-147">取消分配自动程序电话号码</span><span class="sxs-lookup"><span data-stu-id="5d9b0-147">Unassign a bot phone number</span></span>

<span data-ttu-id="5d9b0-148">使用以下 cmdlet 取消分配电话号码。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-148">Use the following cmdlet to unassign a phone number.</span></span>

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

><span data-ttu-id="5d9b0-149">**注意：** 目前，这仅适用于联机号码，不能直接路由 (DR) 号码。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-149">**Note:** Currently this only works with online numbers and not direct routing (DR) numbers.</span></span> <span data-ttu-id="5d9b0-150">这是一个已知问题。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-150">This is a known issue.</span></span>

## <a name="update-a-bot-phone-number"></a><span data-ttu-id="5d9b0-151">更新自动程序电话号码</span><span class="sxs-lookup"><span data-stu-id="5d9b0-151">Update a bot phone number</span></span>

<span data-ttu-id="5d9b0-152">取消分配号码后，可以通过以下 cmdlet 为自动程序分配不同的号码。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-152">After unassigning the number, you can assign a different number to the bot by using the following cmdlet.</span></span>

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a><span data-ttu-id="5d9b0-153">另请参阅</span><span class="sxs-lookup"><span data-stu-id="5d9b0-153">See also</span></span>

- <span data-ttu-id="5d9b0-154">[事件机器人示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot)。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-154">[Incident bot sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot).</span></span> 
 - <span data-ttu-id="5d9b0-155">若要详细了解如何部署，请参阅 [部署示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample)。</span><span class="sxs-lookup"><span data-stu-id="5d9b0-155">For details about how to deploy, see [Deploying the sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample).</span></span>
