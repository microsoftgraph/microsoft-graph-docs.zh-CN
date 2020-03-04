---
title: 使用 Microsoft Graph 通信 API
description: Microsoft Graph 通信 API 通过启用语音和视频功能，为应用和服务与用户的互动方式添加了新的维度。
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 7869ac59f84f266542254fd0c8fc8ea97ee4815d
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394580"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="a9ee8-103">使用 Microsoft Graph 通信 API</span><span class="sxs-lookup"><span data-stu-id="a9ee8-103">Working with the communications API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9ee8-104">Microsoft Graph 通信 API 通过在应用和服务中启用核心通信功能，为你或你的组织与其他用户交互的方式添加了新的维度。</span><span class="sxs-lookup"><span data-stu-id="a9ee8-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="a9ee8-105">可使用此 API 接听电话、创建和检索会议坐标和查看用户的状态。</span><span class="sxs-lookup"><span data-stu-id="a9ee8-105">You can use this API to create and receive calls, create and retrieve meeting coordinates, and check users' presence.</span></span>

<span data-ttu-id="a9ee8-106">可使用通信 API 构建服务应用程序（机器人），它们在通话中充当参与者，代表用户创建和检索会议并检查出席状态和活动。</span><span class="sxs-lookup"><span data-stu-id="a9ee8-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users and to check their presence availability and activity.</span></span>
<span data-ttu-id="a9ee8-107">此 API 提供了通话功能，还可用于创建和检索联机会议。</span><span class="sxs-lookup"><span data-stu-id="a9ee8-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="a9ee8-108">可将服务应用程序（机器人）与此 API 搭配使用，其中机器人可在 VoIP 通话或 Microsoft Teams 会议中充当参与者等等。</span><span class="sxs-lookup"><span data-stu-id="a9ee8-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="a9ee8-109">授权</span><span class="sxs-lookup"><span data-stu-id="a9ee8-109">Authorization</span></span>

<span data-ttu-id="a9ee8-110">需要以下[权限](/graph/permissions-reference#calls-permissions) 之一才能访问通信 API。</span><span class="sxs-lookup"><span data-stu-id="a9ee8-110">One of the following [permissions](/graph/permissions-reference#calls-permissions) is required to access the communications API.</span></span> <span data-ttu-id="a9ee8-111">需要由管理员授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="a9ee8-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="a9ee8-112">方案</span><span class="sxs-lookup"><span data-stu-id="a9ee8-112">Scenario</span></span>                 | <span data-ttu-id="a9ee8-113">权限</span><span class="sxs-lookup"><span data-stu-id="a9ee8-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="a9ee8-114">通话</span><span class="sxs-lookup"><span data-stu-id="a9ee8-114">Calling</span></span>                 | <span data-ttu-id="a9ee8-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="a9ee8-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="a9ee8-116">会议</span><span class="sxs-lookup"><span data-stu-id="a9ee8-116">Meetings</span></span>                 | <span data-ttu-id="a9ee8-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9ee8-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |
| <span data-ttu-id="a9ee8-118">状态</span><span class="sxs-lookup"><span data-stu-id="a9ee8-118">Presence</span></span>                 | <span data-ttu-id="a9ee8-119">状态.阅读，状态.阅读.全部</span><span class="sxs-lookup"><span data-stu-id="a9ee8-119">Presence.Read, Presence.Read.All</span></span> |
| <span data-ttu-id="a9ee8-120">通话记录</span><span class="sxs-lookup"><span data-stu-id="a9ee8-120">Call records</span></span>             | <span data-ttu-id="a9ee8-121">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9ee8-121">CallRecords.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="a9ee8-122">常见用例</span><span class="sxs-lookup"><span data-stu-id="a9ee8-122">Common use cases</span></span>

<span data-ttu-id="a9ee8-123">下表列出了通信 API 的一些常见用例。</span><span class="sxs-lookup"><span data-stu-id="a9ee8-123">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="a9ee8-124">用例</span><span class="sxs-lookup"><span data-stu-id="a9ee8-124">Use cases</span></span>                         | <span data-ttu-id="a9ee8-125">REST 资源</span><span class="sxs-lookup"><span data-stu-id="a9ee8-125">REST resources</span></span>                                 | <span data-ttu-id="a9ee8-126">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a9ee8-126">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="a9ee8-127">创建并键入一对一通话和群组通话</span><span class="sxs-lookup"><span data-stu-id="a9ee8-127">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="a9ee8-128">通话</span><span class="sxs-lookup"><span data-stu-id="a9ee8-128">Call</span></span>](/graph/api/resources/call?view=graph-rest-beta)| [<span data-ttu-id="a9ee8-129">通话方法</span><span class="sxs-lookup"><span data-stu-id="a9ee8-129">Methods for calls</span></span>](/graph/api/resources/call?view=graph-rest-beta#methods)|
|<span data-ttu-id="a9ee8-130">IVR 通话</span><span class="sxs-lookup"><span data-stu-id="a9ee8-130">IVR calls</span></span>   |     | [<span data-ttu-id="a9ee8-131">IVR 方法</span><span class="sxs-lookup"><span data-stu-id="a9ee8-131">Methods for IVR</span></span>](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta)
| <span data-ttu-id="a9ee8-132">通话控制（参与者）</span><span class="sxs-lookup"><span data-stu-id="a9ee8-132">Call controls (participant)</span></span> | [<span data-ttu-id="a9ee8-133">参与者</span><span class="sxs-lookup"><span data-stu-id="a9ee8-133">Participant</span></span>](/graph/api/resources/participant?view=graph-rest-beta)   ||
|<span data-ttu-id="a9ee8-134">会议</span><span class="sxs-lookup"><span data-stu-id="a9ee8-134">Meetings</span></span>|[<span data-ttu-id="a9ee8-135">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="a9ee8-135">onlineMeeting</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-beta)| [<span data-ttu-id="a9ee8-136">会议方法</span><span class="sxs-lookup"><span data-stu-id="a9ee8-136">Methods for meetings</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-beta#methods)|
|<span data-ttu-id="a9ee8-137">状态</span><span class="sxs-lookup"><span data-stu-id="a9ee8-137">Presence</span></span> | [<span data-ttu-id="a9ee8-138">状态</span><span class="sxs-lookup"><span data-stu-id="a9ee8-138">presence</span></span>](/graph/api/resources/presence) | [<span data-ttu-id="a9ee8-139">出席方式</span><span class="sxs-lookup"><span data-stu-id="a9ee8-139">Methods for presence</span></span>](/graph/api/resources/presence#methods) |
| <span data-ttu-id="a9ee8-140">检索通话记录</span><span class="sxs-lookup"><span data-stu-id="a9ee8-140">Retrieving call records</span></span> | [<span data-ttu-id="a9ee8-141">callRecord</span><span class="sxs-lookup"><span data-stu-id="a9ee8-141">callRecord</span></span>](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta) | [<span data-ttu-id="a9ee8-142">Webhook 订阅</span><span class="sxs-lookup"><span data-stu-id="a9ee8-142">Webhook subscriptions</span></span>](/graph/api/resources/webhooks?view=graph-rest-beta) |

## <a name="common-properties"></a><span data-ttu-id="a9ee8-143">通用属性</span><span class="sxs-lookup"><span data-stu-id="a9ee8-143">Common properties</span></span>

| <span data-ttu-id="a9ee8-144">资源</span><span class="sxs-lookup"><span data-stu-id="a9ee8-144">Resource</span></span>                | <span data-ttu-id="a9ee8-145">属性</span><span class="sxs-lookup"><span data-stu-id="a9ee8-145">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="a9ee8-146">通话</span><span class="sxs-lookup"><span data-stu-id="a9ee8-146">call</span></span>                               | [<span data-ttu-id="a9ee8-147">通话属性</span><span class="sxs-lookup"><span data-stu-id="a9ee8-147">call properties</span></span>](/graph/api/resources/call?view=graph-rest-beta#properties)  |
| <span data-ttu-id="a9ee8-148">参与者</span><span class="sxs-lookup"><span data-stu-id="a9ee8-148">participant</span></span>                         | [<span data-ttu-id="a9ee8-149">参与者属性</span><span class="sxs-lookup"><span data-stu-id="a9ee8-149">participant properties</span></span>](/graph/api/resources/participant?view=graph-rest-beta#properties) |
| <span data-ttu-id="a9ee8-150">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="a9ee8-150">onlineMeeting</span></span>                            | [<span data-ttu-id="a9ee8-151">onlineMeeting 属性</span><span class="sxs-lookup"><span data-stu-id="a9ee8-151">onlineMeeting properties</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-beta#properties)                     |
| <span data-ttu-id="a9ee8-152">状态</span><span class="sxs-lookup"><span data-stu-id="a9ee8-152">presence</span></span> | [<span data-ttu-id="a9ee8-153">状态属性</span><span class="sxs-lookup"><span data-stu-id="a9ee8-153">presence properties</span></span>](/graph/api/resources/presence#properties) |
| <span data-ttu-id="a9ee8-154">callRecord</span><span class="sxs-lookup"><span data-stu-id="a9ee8-154">callRecord</span></span> | [<span data-ttu-id="a9ee8-155">callRecord 属性</span><span class="sxs-lookup"><span data-stu-id="a9ee8-155">callRecord properties</span></span>](/graph/api/resources/callrecords-callrecord#properties) |

## <a name="see-also"></a><span data-ttu-id="a9ee8-156">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a9ee8-156">See also</span></span>

- [<span data-ttu-id="a9ee8-157">通信 API 示例</span><span class="sxs-lookup"><span data-stu-id="a9ee8-157">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="a9ee8-158">通信信号 SDK</span><span class="sxs-lookup"><span data-stu-id="a9ee8-158">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls/1.0.0-prerelease.494)
- [<span data-ttu-id="a9ee8-159">通信媒体 SDK</span><span class="sxs-lookup"><span data-stu-id="a9ee8-159">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media/1.0.0-prerelease.494)
