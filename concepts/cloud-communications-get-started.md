---
title: 云通信入门
description: 了解如何使用机器人响应客户的需求并促进协作。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: a1c2ff420df58be8345924c2c6622f7cc6647551
ms.sourcegitcommit: db3d2c6db8dd8f8cc14bdcebb2904d5e056a73e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/20/2021
ms.locfileid: "52579681"
---
# <a name="get-started-with-cloud-communications"></a><span data-ttu-id="7bdfb-103">云通信入门</span><span class="sxs-lookup"><span data-stu-id="7bdfb-103">Get started with cloud communications</span></span>

<span data-ttu-id="7bdfb-104">Microsoft 中的云通信 API Graph通过各种通信相关功能（如通话和联机会议）为应用和服务如何与用户交互添加了新的维度。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-104">The cloud communications APIs in Microsoft Graph add a new dimension to how your apps and services interact with users through various communications related features, such as calling and online meetings.</span></span> <span data-ttu-id="7bdfb-105">本文介绍如何使用机器人响应客户的需求并促进协作。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-105">This article describes how you can use bots to respond to your customers' needs and facilitate collaboration.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7bdfb-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7bdfb-106">Prerequisites</span></span>

<span data-ttu-id="7bdfb-107">在开始使用之前，熟悉以下内容会很有帮助：</span><span class="sxs-lookup"><span data-stu-id="7bdfb-107">Before  you get started, it will be helpful to familiarize yourself with the following:</span></span>

- <span data-ttu-id="7bdfb-108">[Azure Active Directory (](/azure/active-directory/fundamentals/active-directory-whatis) Azure AD) 服务如何帮助员工登录和访问资源。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-108">[Azure Active Directory](/azure/active-directory/fundamentals/active-directory-whatis) (Azure AD) and how the service helps employees sign in and access resources.</span></span>
- <span data-ttu-id="7bdfb-109">[Azure Bot 服务](/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0)及其功能。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-109">The [Azure Bot Service](/azure/bot-service/bot-service-overview-introduction?view=azure-bot-service-3.0) and its capabilities.</span></span>

## <a name="register-a-bot"></a><span data-ttu-id="7bdfb-110">注册自动程序</span><span class="sxs-lookup"><span data-stu-id="7bdfb-110">Register a bot</span></span>

<span data-ttu-id="7bdfb-111">术语"服务应用程序"和"bot"可以互换使用。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-111">The terms "service application" and "bot" can be used interchangeably.</span></span> <span data-ttu-id="7bdfb-112">可以直接通过 Azure 门户创建自动程序 [，](https://azure.microsoft.com/features/azure-portal/) 也可以注册未托管在 Azure 上的自动程序。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-112">You can either create a bot through the [Azure portal](https://azure.microsoft.com/features/azure-portal/) directly or register a bot that isn't hosted on Azure.</span></span> <span data-ttu-id="7bdfb-113">有关机器人注册过程的更多详细信息，请参阅 [注册呼叫机器人](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html)。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-113">For more details about the bot registration process, see [Registering a calling bot](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/register-calling-bot.html).</span></span> 

<span data-ttu-id="7bdfb-114">为了在以后简化操作，了解 Azure AD 中 [不同类型的权限非常有用](/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions) 。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-114">To make things easier later, it's helpful to understand the different [types of permissions](/azure/active-directory/develop/v1-permissions-and-consent#types-of-permissions) within Azure AD.</span></span> <span data-ttu-id="7bdfb-115">具有委派权限的应用需要登录用户。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-115">Apps with delegated permissions require a signed-in user.</span></span> <span data-ttu-id="7bdfb-116">基于应用程序的权限不需要登录用户，通常可以作为后台服务运行。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-116">Application-based permissions don't need a signed-in user, and can often run as a background service.</span></span>

<span data-ttu-id="7bdfb-117">注册自动程序后，如果你想要将机器人添加到[Microsoft Teams，请确保](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot)你了解如何使用[app Studio](/microsoftteams/platform/get-started/get-started-app-studio)并定义所需的元数据。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-117">After you register your bot, if you'd like to [add your bot to Microsoft Teams](/microsoftteams/platform/concepts/calls-and-meetings/registering-calling-bot), make sure you understand how to use [app studio](/microsoftteams/platform/get-started/get-started-app-studio) and define the required metadata.</span></span>

## <a name="manage-the-state-of-the-bot"></a><span data-ttu-id="7bdfb-118">管理自动程序的状态</span><span class="sxs-lookup"><span data-stu-id="7bdfb-118">Manage the state of the bot</span></span>

<span data-ttu-id="7bdfb-119">注册自动程序后，决定是希望基于音频和视频的媒体是应用程序托管的还是 [服务托管的](cloud-communications-media.md)。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-119">After you register your bot, decide whether you want your audio and video-based media to be [application-hosted or service-hosted](cloud-communications-media.md).</span></span> <span data-ttu-id="7bdfb-120">在高级别上，这涉及到决定是否要访问原始媒体实时流。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-120">At a high level, this involves deciding whether or not you want to access a live-stream of raw media.</span></span>

<span data-ttu-id="7bdfb-121">接下来，你可以决定是最适合自动程序是有 [状态还是无状态](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html)。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-121">Next, you can decide whether it's best for your bot to be [stateful or stateless](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/calls/StateManagement.html).</span></span>

### <a name="stateless-bots"></a><span data-ttu-id="7bdfb-122">无状态机器人</span><span class="sxs-lookup"><span data-stu-id="7bdfb-122">Stateless bots</span></span>

<span data-ttu-id="7bdfb-123">任何虚拟机都可以处理任何自动程序实例，这意味着如果一台计算机关闭，另一台计算机可以处理它。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-123">Any virtual machine can handle any bot instance, which means that if one machine goes down, another can take care of it.</span></span> <span data-ttu-id="7bdfb-124">这使得解决方案具有弹性。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-124">This makes for a resilient solution.</span></span>

<span data-ttu-id="7bdfb-125">另一方面，共享缓存（如 REDIS）需要可供所有虚拟机访问。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-125">On the other hand, a shared cache, such as REDIS, needs to be accessible to all the virtual machines.</span></span>

### <a name="stateful-bots"></a><span data-ttu-id="7bdfb-126">有状态自动程序</span><span class="sxs-lookup"><span data-stu-id="7bdfb-126">Stateful bots</span></span>

<span data-ttu-id="7bdfb-127">虚拟机一次只能处理一个自动程序实例。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-127">A virtual machine can handle only one bot instance at a time.</span></span> <span data-ttu-id="7bdfb-128">由于所有状态都位于一台计算机中，因此没有任何额外的内存检查或 REDIS 缓存检查。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-128">Because all the states are on one machine, there aren't any extra memory checks or REDIS cache checks.</span></span>

<span data-ttu-id="7bdfb-129">缺点是，由于自动程序实例仅位于一台计算机中，因此它无法复原。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-129">The drawback is that because the bot instance is just on one machine, it isn't as resilient.</span></span>

><span data-ttu-id="7bdfb-130">**注意：** 服务托管的媒体机器人可以是有状态或无状态的。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-130">**Note:** Service-hosted media bots can be stateful or stateless.</span></span> <span data-ttu-id="7bdfb-131">应用程序托管的媒体机器人必须具有状态，才能使用[Bot Media SDK。](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media)</span><span class="sxs-lookup"><span data-stu-id="7bdfb-131">Application-hosted media bots must be stateful in order to use the [Bot Media SDK](https://www.nuget.org/packages/Microsoft.Skype.Bots.Media).</span></span>

## <a name="use-the-sdks"></a><span data-ttu-id="7bdfb-132">使用 SDK</span><span class="sxs-lookup"><span data-stu-id="7bdfb-132">Use the SDKs</span></span>

<span data-ttu-id="7bdfb-133">以下 SDK 可用于C#。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-133">The following SDKs are available in C#.</span></span> <span data-ttu-id="7bdfb-134">我们将在未来提供对其他语言的支持。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-134">We will provide support for other languages in the future.</span></span>

- <span data-ttu-id="7bdfb-135">如果你使用的是无状态 **机器人**，请安装 [Graph通信核心 SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core)。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-135">If you're using **stateless** bots, install the [Graph Communications Core SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Core).</span></span>
- <span data-ttu-id="7bdfb-136">如果你使用的是有状态 **机器人**，请安装 Graph [Communications Calling SDK。](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)</span><span class="sxs-lookup"><span data-stu-id="7bdfb-136">If you're using **stateful** bots, install the [Graph Communications Calling SDK](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls).</span></span>

## <a name="examples"></a><span data-ttu-id="7bdfb-137">示例</span><span class="sxs-lookup"><span data-stu-id="7bdfb-137">Examples</span></span>

<span data-ttu-id="7bdfb-138">了解如何使用有状态机器人实现不同的方案，例如使用应用程序托管的媒体[](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls)或服务托管的媒体应答传入呼叫。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-138">Learn how to implement different scenarios using stateful bots, such as [answering an incoming call](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/articles/index.html#example-incoming-calls) with either application-hosted or service-hosted media.</span></span>

<span data-ttu-id="7bdfb-139">有关更多示例，请参阅 [通信示例存储库](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html)。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-139">For more examples, see the [Communications samples repository](https://microsoftgraph.github.io/microsoft-graph-comms-samples/docs/index.html).</span></span>

## <a name="privacy-and-compliance"></a><span data-ttu-id="7bdfb-140">隐私与合规性</span><span class="sxs-lookup"><span data-stu-id="7bdfb-140">Privacy and compliance</span></span>

<span data-ttu-id="7bdfb-141">在 API 请求中，不应以任何客户端生成的 ID (（如标头或请求正文中的方案 ID、请求 ID 或其他相关 ID) ）发送敏感数据。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-141">In the requests to our APIs, sensitive data should not be sent in any client-side generated IDs (such as scenario IDs, request IDs, or other correlation IDs) in headers or the request body.</span></span> <span data-ttu-id="7bdfb-142">这些 ID 将记录在服务器端进行诊断。</span><span class="sxs-lookup"><span data-stu-id="7bdfb-142">These IDs will be logged on the server side for diagnostics.</span></span>
