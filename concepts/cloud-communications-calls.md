---
title: 呼叫概述
description: 了解支持的呼叫类型及其用于信号流程的方式。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 8de1f5d890504d9edc63213333f1ea8c4b47282f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871583"
---
# <a name="calls-overview"></a><span data-ttu-id="50fc0-103">呼叫概述</span><span class="sxs-lookup"><span data-stu-id="50fc0-103">Calls overview</span></span>

<span data-ttu-id="50fc0-104">Microsoft Graph 中的云通信 Api 为您的应用程序和服务通过各种通信相关功能（如呼叫和联机会议）与用户进行交互的方式添加了一个新的维度。</span><span class="sxs-lookup"><span data-stu-id="50fc0-104">The cloud communications APIs in Microsoft Graph add a new dimension to how your apps and services interact with users through various communications related features, such as calls and online meetings.</span></span> <span data-ttu-id="50fc0-105">本文介绍了受支持的呼叫类型以及它们如何用于信号流程。</span><span class="sxs-lookup"><span data-stu-id="50fc0-105">This article describes the supported call types and how they're used for the signaling process.</span></span>

## <a name="peer-to-peer-calls"></a><span data-ttu-id="50fc0-106">对等呼叫</span><span class="sxs-lookup"><span data-stu-id="50fc0-106">Peer-to-peer calls</span></span>
<span data-ttu-id="50fc0-107">当一个参与者直接呼叫另一个参与者时，呼叫为对等（P2P）。</span><span class="sxs-lookup"><span data-stu-id="50fc0-107">A call is peer-to-peer (P2P) when one participant is directly calling another participant.</span></span> <span data-ttu-id="50fc0-108">如果机器人呼叫用户，并且用户是指定的唯一呼叫目标，则这是 P2P 呼叫的一个示例。</span><span class="sxs-lookup"><span data-stu-id="50fc0-108">If a bot calls a user, and the user is the only calling target specified, this is an example of a P2P call.</span></span>

![P2P 调用关系图](images/communications-p2p-call.PNG)

<span data-ttu-id="50fc0-110">如果用户想要呼叫机器人，bot 不需要任何其他权限即可响应 P2P 呼叫。</span><span class="sxs-lookup"><span data-stu-id="50fc0-110">If a user wants to call a bot, the bot doesn't need any additional permissions in order to respond to the P2P call.</span></span> <span data-ttu-id="50fc0-111">为了使 bot 能够呼叫用户，它必须具有调用。 Initiate。 P2P 呼叫的所有权限。</span><span class="sxs-lookup"><span data-stu-id="50fc0-111">In order for a bot to call a user, it must have the Calls.Initiate.All permission for a P2P call.</span></span>

## <a name="group-calls"></a><span data-ttu-id="50fc0-112">组调用</span><span class="sxs-lookup"><span data-stu-id="50fc0-112">Group calls</span></span>

<span data-ttu-id="50fc0-113">如果呼叫中有三个或更多参与者，或者在最初创建呼叫时指定了[会议坐标](/graph/api/resources/onlinemeeting)，则会发生组调用。</span><span class="sxs-lookup"><span data-stu-id="50fc0-113">A group call occurs if there are either three or more participants in the call, or if [meeting coordinates](/graph/api/resources/onlinemeeting) were specified when the call was initially created.</span></span> 

<span data-ttu-id="50fc0-114">例如，您可以通过 Microsoft 团队创建组呼叫。</span><span class="sxs-lookup"><span data-stu-id="50fc0-114">You can create a group call through Microsoft Teams, for example.</span></span>

![分组调用关系图](images/communications-group-call.PNG)

<span data-ttu-id="50fc0-116">目前，bot 能够：</span><span class="sxs-lookup"><span data-stu-id="50fc0-116">Currently, bots are able to:</span></span>
- <span data-ttu-id="50fc0-117">创建组调用</span><span class="sxs-lookup"><span data-stu-id="50fc0-117">Create group calls</span></span>
- <span data-ttu-id="50fc0-118">加入现有的组调用</span><span class="sxs-lookup"><span data-stu-id="50fc0-118">Join exisiting group calls</span></span>
- <span data-ttu-id="50fc0-119">邀请其他参与者加入现有的组呼叫</span><span class="sxs-lookup"><span data-stu-id="50fc0-119">Invite other participants into an existing group call</span></span>
- <span data-ttu-id="50fc0-120">被邀请加入现有的组调用</span><span class="sxs-lookup"><span data-stu-id="50fc0-120">Be invited into existing group calls</span></span>

## <a name="see-also"></a><span data-ttu-id="50fc0-121">另请参阅</span><span class="sxs-lookup"><span data-stu-id="50fc0-121">See also</span></span>

- [<span data-ttu-id="50fc0-122">云通信 API 概述</span><span class="sxs-lookup"><span data-stu-id="50fc0-122">Cloud communications API overview</span></span>](cloud-communications-concept-overview.md)
- [<span data-ttu-id="50fc0-123">呼叫权限</span><span class="sxs-lookup"><span data-stu-id="50fc0-123">Permissions for calls</span></span>](/graph/permissions-reference#calls-permissions)
