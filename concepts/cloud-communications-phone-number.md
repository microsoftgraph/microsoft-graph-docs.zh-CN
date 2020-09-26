---
title: 管理机器人的电话号码
description: 本文介绍如何创建可通过电话号码访问的机器人。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 679ee5ac5da1a8754d7517dfb9f35bd9e0a071db
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289370"
---
# <a name="manage-phone-numbers-for-bots"></a><span data-ttu-id="85f89-103">管理机器人的电话号码</span><span class="sxs-lookup"><span data-stu-id="85f89-103">Manage phone numbers for bots</span></span> 

<span data-ttu-id="85f89-104">本文介绍如何创建可通过电话号码访问的机器人。</span><span class="sxs-lookup"><span data-stu-id="85f89-104">This article describes how to create a bot that is reachable through a phone number.</span></span> <span data-ttu-id="85f89-105">在创建你的 bot 时，熟悉以下术语将很有帮助：</span><span class="sxs-lookup"><span data-stu-id="85f89-105">As you create your bot, it will be helpful to be familiar with the following terms:</span></span>

- <span data-ttu-id="85f89-106">**应用程序** –托管在 Azure 上的应用程序（也称为 **bot**）。</span><span class="sxs-lookup"><span data-stu-id="85f89-106">**Application** – An application that is hosted on Azure, also referred to as a **bot**.</span></span>

- <span data-ttu-id="85f89-107">**应用程序实例** –可分配给机器人可使用的电话号码的已禁用用户对象。</span><span class="sxs-lookup"><span data-stu-id="85f89-107">**Application instance** – A disabled-user object that can be assigned to a phone number that can be used by a bot.</span></span> <span data-ttu-id="85f89-108">这也称为 [资源帐户](/microsoftteams/manage-resource-accounts)。</span><span class="sxs-lookup"><span data-stu-id="85f89-108">This is also known as a [resource account](/microsoftteams/manage-resource-accounts).</span></span> <span data-ttu-id="85f89-109">这是可以将电话号码分配给 bot 的唯一方法。</span><span class="sxs-lookup"><span data-stu-id="85f89-109">This is the only way a phone number can be assigned to a bot.</span></span>

<span data-ttu-id="85f89-110">一个应用程序可以有多个应用程序实例，每个租户可以有多个应用程序实例，如下图所示。</span><span class="sxs-lookup"><span data-stu-id="85f89-110">One application can have multiple application instances, and each tenant can have multiple application instances, as shown in the following image.</span></span>

![显示具有一个或多个应用程序实例的租户的电话号码的图像](images/communications-app-tenant.PNG)

## <a name="prerequisite---register-a-bot"></a><span data-ttu-id="85f89-112">先决条件-注册 bot</span><span class="sxs-lookup"><span data-stu-id="85f89-112">Prerequisite - Register a bot</span></span>
<span data-ttu-id="85f89-113">若要开始，请按照说明 [注册呼叫机器人](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html)。</span><span class="sxs-lookup"><span data-stu-id="85f89-113">To get started, follow the instructions to [register a calling bot](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html).</span></span> <span data-ttu-id="85f89-114">你将需要在代码中使用的配置值（如 bot ID、Microsoft app ID 和 Microsoft 应用密码）。</span><span class="sxs-lookup"><span data-stu-id="85f89-114">You’ll need config values such as bot ID, Microsoft app ID, and Microsoft app password to use in your code.</span></span>

<span data-ttu-id="85f89-115">向你的 bot 添加以下权限。</span><span class="sxs-lookup"><span data-stu-id="85f89-115">Add the following permissions to your bot.</span></span> <span data-ttu-id="85f89-116">租户管理员还需要同意这些权限：</span><span class="sxs-lookup"><span data-stu-id="85f89-116">A tenant admin needs to consent to these permissions as well:</span></span>

- <span data-ttu-id="85f89-117">Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="85f89-117">Calls.AccessMedia.All</span></span>
- <span data-ttu-id="85f89-118">Calls.Initiate.All</span><span class="sxs-lookup"><span data-stu-id="85f89-118">Calls.Initiate.All</span></span>
- <span data-ttu-id="85f89-119">Calls.JoinGroupCall.All</span><span class="sxs-lookup"><span data-stu-id="85f89-119">Calls.JoinGroupCall.All</span></span>
- <span data-ttu-id="85f89-120">JoinGroupCallAsGuest</span><span class="sxs-lookup"><span data-stu-id="85f89-120">Calls.JoinGroupCallAsGuest.All</span></span>

<span data-ttu-id="85f89-121">有关与呼叫相关的权限的详细信息，请参阅 [权限参考](permissions-reference.md#calls-permissions)。</span><span class="sxs-lookup"><span data-stu-id="85f89-121">For more information about call-related permissions, see the [Permissions reference](permissions-reference.md#calls-permissions).</span></span>


## <a name="assign-a-phone-number-to-your-bot"></a><span data-ttu-id="85f89-122">将电话号码分配给你的机器人</span><span class="sxs-lookup"><span data-stu-id="85f89-122">Assign a phone number to your bot</span></span>

<span data-ttu-id="85f89-123">为你的 bot 分配电话号码包括三个步骤：</span><span class="sxs-lookup"><span data-stu-id="85f89-123">Assigning a phone number to your bot involves three steps:</span></span>

1.  <span data-ttu-id="85f89-124">创建应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="85f89-124">Create an application instance.</span></span>
2.  <span data-ttu-id="85f89-125">将虚拟用户许可证分配给应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="85f89-125">Assign a virtual user license to your application instance.</span></span>
3.  <span data-ttu-id="85f89-126">仅 (租户管理员) 向应用程序实例分配电话号码。</span><span class="sxs-lookup"><span data-stu-id="85f89-126">Assign a phone number to the application instance (only tenant admin).</span></span>

### <a name="create-an-application-instance"></a><span data-ttu-id="85f89-127">创建应用程序实例</span><span class="sxs-lookup"><span data-stu-id="85f89-127">Create an application instance</span></span>

<span data-ttu-id="85f89-128">如果尚未安装，租户管理员需要为 PowerShell 安装 [Skype For Business Online 模块](https://www.microsoft.com/download/details.aspx?id=39366) 。</span><span class="sxs-lookup"><span data-stu-id="85f89-128">If it hasn't been installed already, a tenant admin needs to install the [Skype for Business Online Module](https://www.microsoft.com/download/details.aspx?id=39366) for PowerShell.</span></span> <span data-ttu-id="85f89-129">租户管理员必须先使用其凭据登录，然后才能运行 cmdlet。</span><span class="sxs-lookup"><span data-stu-id="85f89-129">The tenant admin must sign in using their credentials before running the cmdlet.</span></span>

<span data-ttu-id="85f89-130">若要创建新的应用程序实例，租户管理员需要运行以下 cmdlet。</span><span class="sxs-lookup"><span data-stu-id="85f89-130">To create a new application instance, the tenant admin runs the following cmdlet.</span></span>

`PS C:\> New-CsOnlineApplicationInstance -UserPrincipalName <user@contoso.com> -ApplicationId “<app_id>” -DisplayName "<bot_display_name>"`

<span data-ttu-id="85f89-131">创建应用程序实例时，请使用 sync cmdlet。</span><span class="sxs-lookup"><span data-stu-id="85f89-131">When the application instance is created, use the sync cmdlet.</span></span>

`PS C:\> Sync-CsOnlineApplicationInstance -ObjectId <application_instance_id>`

### <a name="assign-a-virtual-user-license-to-your-application-instance"></a><span data-ttu-id="85f89-132">将虚拟用户许可证分配给应用程序实例</span><span class="sxs-lookup"><span data-stu-id="85f89-132">Assign a virtual user license to your application instance</span></span>

<span data-ttu-id="85f89-133">将虚拟用户许可证分配给应用程序实例。</span><span class="sxs-lookup"><span data-stu-id="85f89-133">Assign a virtual user license to your application instance.</span></span> <span data-ttu-id="85f89-134">有关详细信息，请参阅 [电话系统虚拟用户许可证](/microsoftteams/teams-add-on-licensing/virtual-user)。</span><span class="sxs-lookup"><span data-stu-id="85f89-134">For details, see [Phone system virtual user license](/microsoftteams/teams-add-on-licensing/virtual-user).</span></span>

### <a name="assign-a-phone-number-to-the-application-instance-only-tenant-admin"></a><span data-ttu-id="85f89-135">仅将电话号码分配给应用程序实例 (仅租户管理员) </span><span class="sxs-lookup"><span data-stu-id="85f89-135">Assign a phone number to the application instance (only tenant admin)</span></span>

<span data-ttu-id="85f89-136">若要将电话号码分配给应用程序实例，租户管理员请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="85f89-136">To assign the phone number to the application instance, the tenant admin:</span></span>

1. <span data-ttu-id="85f89-137">以租户管理员身份登录到团队管理中心。</span><span class="sxs-lookup"><span data-stu-id="85f89-137">Signs in to the Teams admin center as a tenant admin.</span></span>
2. <span data-ttu-id="85f89-138">转到 "**团队管理员中心**"  >  **语音**  >  **电话号码**。</span><span class="sxs-lookup"><span data-stu-id="85f89-138">Goes to **Teams Admin center** > **Voice** > **Phone Numbers**.</span></span>
3. <span data-ttu-id="85f89-139">使用以下 cmdlet 将服务电话号码分配 (+ 11D 格式) 。</span><span class="sxs-lookup"><span data-stu-id="85f89-139">Assigns a service phone number (+11D format) using the following cmdlet.</span></span>

  `PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <phone_number>`

## <a name="unassign-a-bot-phone-number"></a><span data-ttu-id="85f89-140">取消分配机器人电话号码</span><span class="sxs-lookup"><span data-stu-id="85f89-140">Unassign a bot phone number</span></span>

<span data-ttu-id="85f89-141">使用以下 cmdlet 取消分配电话号码。</span><span class="sxs-lookup"><span data-stu-id="85f89-141">Use the following cmdlet to unassign a phone number.</span></span>

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber $null`

><span data-ttu-id="85f89-142">**注意：** 目前，这仅适用于联机号码，而不是直接路由 (DR) 号码。</span><span class="sxs-lookup"><span data-stu-id="85f89-142">**Note:** Currently this only works with online numbers and not direct routing (DR) numbers.</span></span> <span data-ttu-id="85f89-143">这是一个已知问题。</span><span class="sxs-lookup"><span data-stu-id="85f89-143">This is a known issue.</span></span>

## <a name="update-a-bot-phone-number"></a><span data-ttu-id="85f89-144">更新机器人电话号码</span><span class="sxs-lookup"><span data-stu-id="85f89-144">Update a bot phone number</span></span>

<span data-ttu-id="85f89-145">取消分配号码后，可以使用以下 cmdlet 为 bot 分配其他号码。</span><span class="sxs-lookup"><span data-stu-id="85f89-145">After unassigning the number, you can assign a different number to the bot by using the following cmdlet.</span></span>

`PS C:\> Set-CsOnlineVoiceApplicationInstance -Identity <user@contoso.com> -TelephoneNumber <new phone_number>`

## <a name="see-also"></a><span data-ttu-id="85f89-146">另请参阅</span><span class="sxs-lookup"><span data-stu-id="85f89-146">See also</span></span>

- <span data-ttu-id="85f89-147">[事件 bot 示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot)。</span><span class="sxs-lookup"><span data-stu-id="85f89-147">[Incident bot sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples/IncidentBot).</span></span> 
 - <span data-ttu-id="85f89-148">有关如何部署的详细信息，请参阅 [部署示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample)。</span><span class="sxs-lookup"><span data-stu-id="85f89-148">For details about how to deploy, see [Deploying the sample](https://github.com/microsoftgraph/microsoft-graph-comms-samples/blob/master/Samples/BetaSamples/RemoteMediaSamples/README.md#deploying-the-sample).</span></span>