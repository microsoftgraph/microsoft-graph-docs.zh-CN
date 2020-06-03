---
title: 使用 Microsoft Graph 通信 API
description: Microsoft Graph 通信 API 通过启用语音和视频功能，为应用和服务与用户的互动方式添加了新的维度。
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: b0337dfe620318482f3cc400512d5c381bf123a9
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44491880"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="44a4d-103">使用 Microsoft Graph 通信 API</span><span class="sxs-lookup"><span data-stu-id="44a4d-103">Working with the communications API in Microsoft Graph</span></span>

<span data-ttu-id="44a4d-104">Microsoft Graph 通信 API 通过在应用和服务中启用核心通信功能，为你或你的组织与其他用户交互的方式添加了新的维度。</span><span class="sxs-lookup"><span data-stu-id="44a4d-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="44a4d-105">可使用此 API 接听电话、创建和检索会议坐标。</span><span class="sxs-lookup"><span data-stu-id="44a4d-105">You can use this API to create and receive calls as well as create and retrieve meeting coordinates.</span></span>

<span data-ttu-id="44a4d-106">可使用通信 API 构建服务应用程序（机器人），它们在通话中充当参与者，并代表用户创建和检索会议。</span><span class="sxs-lookup"><span data-stu-id="44a4d-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users.</span></span>
<span data-ttu-id="44a4d-107">此 API 提供了通话功能，还可用于创建和检索联机会议。</span><span class="sxs-lookup"><span data-stu-id="44a4d-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="44a4d-108">可将服务应用程序（机器人）与此 API 搭配使用，其中机器人可在 VoIP 通话或 Microsoft Teams 会议中充当参与者等等。</span><span class="sxs-lookup"><span data-stu-id="44a4d-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="44a4d-109">授权</span><span class="sxs-lookup"><span data-stu-id="44a4d-109">Authorization</span></span>

<span data-ttu-id="44a4d-110">需要以下[权限](https://docs.microsoft.com/graph/permissions-reference#calls-permissions) 之一才能访问通信 API。</span><span class="sxs-lookup"><span data-stu-id="44a4d-110">One of the following [permissions](https://docs.microsoft.com/graph/permissions-reference#calls-permissions) is required to access the communications API.</span></span> <span data-ttu-id="44a4d-111">需要由管理员授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="44a4d-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="44a4d-112">方案</span><span class="sxs-lookup"><span data-stu-id="44a4d-112">Scenario</span></span>                 | <span data-ttu-id="44a4d-113">权限</span><span class="sxs-lookup"><span data-stu-id="44a4d-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="44a4d-114">通话</span><span class="sxs-lookup"><span data-stu-id="44a4d-114">Calling</span></span>                 | <span data-ttu-id="44a4d-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="44a4d-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="44a4d-116">会议</span><span class="sxs-lookup"><span data-stu-id="44a4d-116">Meetings</span></span>                 | <span data-ttu-id="44a4d-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="44a4d-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |
| <span data-ttu-id="44a4d-118">通话记录</span><span class="sxs-lookup"><span data-stu-id="44a4d-118">Call records</span></span>             | <span data-ttu-id="44a4d-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="44a4d-119">CallRecords.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="44a4d-120">常见用例</span><span class="sxs-lookup"><span data-stu-id="44a4d-120">Common use cases</span></span>

<span data-ttu-id="44a4d-121">下表列出了通信 API 的一些常见用例。</span><span class="sxs-lookup"><span data-stu-id="44a4d-121">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="44a4d-122">用例</span><span class="sxs-lookup"><span data-stu-id="44a4d-122">Use cases</span></span>                         | <span data-ttu-id="44a4d-123">REST 资源</span><span class="sxs-lookup"><span data-stu-id="44a4d-123">REST resources</span></span>                                 | <span data-ttu-id="44a4d-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="44a4d-124">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="44a4d-125">创建并键入一对一通话和群组通话</span><span class="sxs-lookup"><span data-stu-id="44a4d-125">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="44a4d-126">通话</span><span class="sxs-lookup"><span data-stu-id="44a4d-126">Call</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0)| [<span data-ttu-id="44a4d-127">通话方法</span><span class="sxs-lookup"><span data-stu-id="44a4d-127">Methods for calls</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#methods)| 
|<span data-ttu-id="44a4d-128">IVR 通话</span><span class="sxs-lookup"><span data-stu-id="44a4d-128">IVR calls</span></span>   |     | [<span data-ttu-id="44a4d-129">IVR 方法</span><span class="sxs-lookup"><span data-stu-id="44a4d-129">Methods for IVR</span></span>](https://docs.microsoft.com/graph/api/resources/calls-api-ivr-overview?view=graph-rest-v1.0)
| <span data-ttu-id="44a4d-130">通话控制（参与者）</span><span class="sxs-lookup"><span data-stu-id="44a4d-130">Call controls (participant)</span></span> | [<span data-ttu-id="44a4d-131">参与者</span><span class="sxs-lookup"><span data-stu-id="44a4d-131">Participant</span></span>](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0)   ||
|<span data-ttu-id="44a4d-132">会议</span><span class="sxs-lookup"><span data-stu-id="44a4d-132">Meetings</span></span>|[<span data-ttu-id="44a4d-133">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="44a4d-133">onlineMeeting</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0)| [<span data-ttu-id="44a4d-134">会议方法</span><span class="sxs-lookup"><span data-stu-id="44a4d-134">Methods for meetings</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#methods)|
| <span data-ttu-id="44a4d-135">检索通话记录</span><span class="sxs-lookup"><span data-stu-id="44a4d-135">Retrieving call records</span></span> | [<span data-ttu-id="44a4d-136">callRecord</span><span class="sxs-lookup"><span data-stu-id="44a4d-136">callRecord</span></span>](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) | [<span data-ttu-id="44a4d-137">Webhook 订阅</span><span class="sxs-lookup"><span data-stu-id="44a4d-137">Webhook subscriptions</span></span>](/graph/api/resources/webhooks?view=graph-rest-1.0) |

## <a name="common-properties"></a><span data-ttu-id="44a4d-138">通用属性</span><span class="sxs-lookup"><span data-stu-id="44a4d-138">Common properties</span></span>

| <span data-ttu-id="44a4d-139">资源</span><span class="sxs-lookup"><span data-stu-id="44a4d-139">Resource</span></span>                | <span data-ttu-id="44a4d-140">属性</span><span class="sxs-lookup"><span data-stu-id="44a4d-140">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="44a4d-141">通话</span><span class="sxs-lookup"><span data-stu-id="44a4d-141">call</span></span>                               | [<span data-ttu-id="44a4d-142">通话属性</span><span class="sxs-lookup"><span data-stu-id="44a4d-142">call properties</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#properties)  |
| <span data-ttu-id="44a4d-143">参与者</span><span class="sxs-lookup"><span data-stu-id="44a4d-143">participant</span></span>                         | [<span data-ttu-id="44a4d-144">参与者属性</span><span class="sxs-lookup"><span data-stu-id="44a4d-144">participant properties</span></span>](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0#properties) |
| <span data-ttu-id="44a4d-145">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="44a4d-145">onlineMeeting</span></span>                            | [<span data-ttu-id="44a4d-146">onlineMeeting 属性</span><span class="sxs-lookup"><span data-stu-id="44a4d-146">onlineMeeting properties</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#properties)                     |
| <span data-ttu-id="44a4d-147">callRecord</span><span class="sxs-lookup"><span data-stu-id="44a4d-147">callRecord</span></span> | [<span data-ttu-id="44a4d-148">callRecord 属性</span><span class="sxs-lookup"><span data-stu-id="44a4d-148">callRecord properties</span></span>](/graph/api/resources/callrecords-callrecord#properties) |

## <a name="whats-new"></a><span data-ttu-id="44a4d-149">最近更新</span><span class="sxs-lookup"><span data-stu-id="44a4d-149">What's new</span></span>
<span data-ttu-id="44a4d-150">查找有关此 API 集的[最新新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="44a4d-150">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="see-also"></a><span data-ttu-id="44a4d-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="44a4d-151">See also</span></span>

- [<span data-ttu-id="44a4d-152">通信 API 示例</span><span class="sxs-lookup"><span data-stu-id="44a4d-152">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="44a4d-153">通信信号 SDK</span><span class="sxs-lookup"><span data-stu-id="44a4d-153">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)
- [<span data-ttu-id="44a4d-154">通信媒体 SDK</span><span class="sxs-lookup"><span data-stu-id="44a4d-154">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media)
