---
title: 云通信入门
description: 了解如何使用 bot 来响应客户需求并促进协作。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: ae04e60079a789125dd6a818c19ec625eaac1443
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871577"
---
# <a name="get-started-with-cloud-communications"></a><span data-ttu-id="2c06b-103">云通信入门</span><span class="sxs-lookup"><span data-stu-id="2c06b-103">Get started with cloud communications</span></span>

<span data-ttu-id="2c06b-104">Microsoft Graph 中的云通信 Api 为您的应用和服务如何通过各种通信相关功能（如呼叫和联机会议）与用户进行交互，从而添加了一个新的维度。</span><span class="sxs-lookup"><span data-stu-id="2c06b-104">The cloud communications APIs in Microsoft Graph add a new dimension to how your apps and services interact with users through various communications related features, such as calling and online meetings.</span></span> <span data-ttu-id="2c06b-105">本文介绍如何使用 bot 来响应客户需求并促进协作。</span><span class="sxs-lookup"><span data-stu-id="2c06b-105">This article describes how you can use bots to respond to your customers' needs and facilitate collaboration.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2c06b-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2c06b-106">Prerequisites</span></span>

<span data-ttu-id="2c06b-107">Beore 开始时，熟悉以下内容会很有帮助：</span><span class="sxs-lookup"><span data-stu-id="2c06b-107">Beore  you get started, it will be helpful to familiarize yourself with the following:</span></span>

- <span data-ttu-id="2c06b-108">[Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-whatis) （azure AD）以及服务如何帮助员工登录和访问资源。</span><span class="sxs-lookup"><span data-stu-id="2c06b-108">[Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-whatis) (Azure AD) and how the service helps employees sign in and access resources.</span></span>
- <span data-ttu-id="2c06b-109">[Azure Bot 服务](https://docs.microsoft.com/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0)及其功能。</span><span class="sxs-lookup"><span data-stu-id="2c06b-109">The [Azure Bot Service](https://docs.microsoft.com/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0) and its capabilities.</span></span>

## <a name="register-a-bot"></a><span data-ttu-id="2c06b-110">注册 bot</span><span class="sxs-lookup"><span data-stu-id="2c06b-110">Register a bot</span></span>

<span data-ttu-id="2c06b-111">术语 "服务应用程序" 和 "bot" 可互换使用。</span><span class="sxs-lookup"><span data-stu-id="2c06b-111">The terms "service application" and "bot" can be used interchangeably.</span></span> <span data-ttu-id="2c06b-112">您可以通过[azure 门户](https://azure.microsoft.com/features/azure-portal/)直接创建机器人，也可以注册不在 azure 上托管的 bot。</span><span class="sxs-lookup"><span data-stu-id="2c06b-112">You can either create a bot through the [Azure portal](https://azure.microsoft.com/features/azure-portal/) directly or register a bot that isn't hosted on Azure.</span></span> <span data-ttu-id="2c06b-113">有关 bot 注册过程的更多详细信息，请参阅[注册呼叫机器人](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html)。</span><span class="sxs-lookup"><span data-stu-id="2c06b-113">For more details about the bot registration process, see [Registering a calling bot](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html).</span></span> 

<span data-ttu-id="2c06b-114">为更轻松地执行更多操作，了解 Azure AD 中的不同[类型的权限](https://docs.microsoft.com/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions)非常有用。</span><span class="sxs-lookup"><span data-stu-id="2c06b-114">To make things easier later, it's helpful to understand the different [types of permissions](https://docs.microsoft.com/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions) within Azure AD.</span></span> <span data-ttu-id="2c06b-115">具有委派权限的应用程序需要已登录用户。</span><span class="sxs-lookup"><span data-stu-id="2c06b-115">Apps with delegated permissions require a signed-in user.</span></span> <span data-ttu-id="2c06b-116">基于应用程序的权限不需要登录用户，并且通常可以作为后台服务运行。</span><span class="sxs-lookup"><span data-stu-id="2c06b-116">Application-based permissions don't need a signed-in user, and can often run as a background service.</span></span>

<span data-ttu-id="2c06b-117">注册你的 bot 后，如果你想要[将你的 bot 添加到 Microsoft 团队](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot)，请确保了解如何使用[应用程序 studio](https://docs.microsoft.com/microsoftteams/platform/get-started/get-started-app-studio)并定义所需的元数据。</span><span class="sxs-lookup"><span data-stu-id="2c06b-117">After you register your bot, if you'd like to [add your bot to Microsoft Teams](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot), make sure you understand how to use [app studio](https://docs.microsoft.com/microsoftteams/platform/get-started/get-started-app-studio) and define the required metadata.</span></span>

## <a name="manage-the-state-of-the-bot"></a><span data-ttu-id="2c06b-118">管理机器人的状态</span><span class="sxs-lookup"><span data-stu-id="2c06b-118">Manage the state of the bot</span></span>

<span data-ttu-id="2c06b-119">注册你的 bot 后，决定是希望基于音频和视频的媒体是[应用程序托管的还是托管服务的](cloud-communications-media.md)。</span><span class="sxs-lookup"><span data-stu-id="2c06b-119">After you register your bot, decide whether you want your audio and video-based media to be [application-hosted or service-hosted](cloud-communications-media.md).</span></span> <span data-ttu-id="2c06b-120">从较高的层次来看，这需要决定是否要访问原始媒体的实时流。</span><span class="sxs-lookup"><span data-stu-id="2c06b-120">At a high level, this involves deciding whether or not you want to access a live-stream of raw media.</span></span>

<span data-ttu-id="2c06b-121">接下来，你可以决定是否最适合你的 bot 进行[状态或无状态](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html)。</span><span class="sxs-lookup"><span data-stu-id="2c06b-121">Next, you can decide whether it's best for your bot to be [stateful or stateless](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html).</span></span>

### <a name="stateless-bots"></a><span data-ttu-id="2c06b-122">无状态 bot</span><span class="sxs-lookup"><span data-stu-id="2c06b-122">Stateless bots</span></span>

<span data-ttu-id="2c06b-123">任何虚拟机都可以处理任何 bot 实例，这意味着如果一台计算机出现故障，另一台可能会处理它。</span><span class="sxs-lookup"><span data-stu-id="2c06b-123">Any virtual machine can handle any bot instance, which means that if one machine goes down, another can take care of it.</span></span> <span data-ttu-id="2c06b-124">这将生成弹性解决方案。</span><span class="sxs-lookup"><span data-stu-id="2c06b-124">This makes for a resilient solution.</span></span>

<span data-ttu-id="2c06b-125">另一方面，共享缓存（如 REDIS）需要对所有虚拟机都是可访问的。</span><span class="sxs-lookup"><span data-stu-id="2c06b-125">On the other hand, a shared cache, such as REDIS, needs to be accessible to all the virtual machines.</span></span>

### <a name="stateful-bots"></a><span data-ttu-id="2c06b-126">有状态的 bot</span><span class="sxs-lookup"><span data-stu-id="2c06b-126">Stateful bots</span></span>

<span data-ttu-id="2c06b-127">虚拟机一次只能处理一个 bot 实例。</span><span class="sxs-lookup"><span data-stu-id="2c06b-127">A virtual machine can handle only one bot instance at a time.</span></span> <span data-ttu-id="2c06b-128">由于所有状态都在一台计算机上，因此没有任何额外的内存检查或 REDIS 缓存检查。</span><span class="sxs-lookup"><span data-stu-id="2c06b-128">Because all the states are on one machine, there aren't any extra memory checks or REDIS cache checks.</span></span>

<span data-ttu-id="2c06b-129">缺点是，由于 bot 实例只在一台计算机上，因此不能恢复。</span><span class="sxs-lookup"><span data-stu-id="2c06b-129">The drawback is that because the bot instance is just on one machine, it isn't as resilient.</span></span>

><span data-ttu-id="2c06b-130">**注意：** 服务托管的媒体 bot 可以是有状态的，也可以是无状态的。</span><span class="sxs-lookup"><span data-stu-id="2c06b-130">**Note:** Service-hosted media bots can be stateful or stateless.</span></span> <span data-ttu-id="2c06b-131">应用程序托管的媒体 bot 必须处于状态，才能使用[Bot 媒体 SDK](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media)。</span><span class="sxs-lookup"><span data-stu-id="2c06b-131">Application-hosted media bots must be stateful in order to use the [Bot Media SDK](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media).</span></span>

## <a name="use-the-sdks"></a><span data-ttu-id="2c06b-132">使用 Sdk</span><span class="sxs-lookup"><span data-stu-id="2c06b-132">Use the SDKs</span></span>

<span data-ttu-id="2c06b-133">C # 中提供了以下 Sdk。</span><span class="sxs-lookup"><span data-stu-id="2c06b-133">The following SDKs are available in C#.</span></span> <span data-ttu-id="2c06b-134">我们将在将来为其他语言提供支持。</span><span class="sxs-lookup"><span data-stu-id="2c06b-134">We will provide support for other languages in the future.</span></span>

- <span data-ttu-id="2c06b-135">如果您使用的是**无状态**bot，请安装[GRAPH 通信核心 SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core)。</span><span class="sxs-lookup"><span data-stu-id="2c06b-135">If you're using **stateless** bots, install the [Graph Communications Core SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core).</span></span>
- <span data-ttu-id="2c06b-136">如果您使用的是有**状态**的 bot，请安装[GRAPH 通信呼叫 SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)。</span><span class="sxs-lookup"><span data-stu-id="2c06b-136">If you're using **stateful** bots, install the [Graph Communications Calling SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls).</span></span>

## <a name="examples"></a><span data-ttu-id="2c06b-137">示例</span><span class="sxs-lookup"><span data-stu-id="2c06b-137">Examples</span></span>

<span data-ttu-id="2c06b-138">了解如何使用有状态的 bot 实施不同的方案，例如，使用应用程序托管或服务承载的媒体[应答传入呼叫](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls)。</span><span class="sxs-lookup"><span data-stu-id="2c06b-138">Learn how to implement different scenarios using stateful bots, such as [answering an incoming call](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls) with either application-hosted or service-hosted media.</span></span>

<span data-ttu-id="2c06b-139">有关更多示例，请参阅[通信示例存储库](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html)。</span><span class="sxs-lookup"><span data-stu-id="2c06b-139">For more examples, see the [Communications samples repository](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html).</span></span>
