---
title: 使用 Microsoft Graph 通信 API
description: Microsoft Graph 通信 API 通过启用语音和视频功能，为应用和服务与用户的互动方式添加了新的维度。
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 636eeedb4836a26e5fe2e52683f8baacdb4a8d69
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353250"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="bd9fd-103">使用 Microsoft Graph 通信 API</span><span class="sxs-lookup"><span data-stu-id="bd9fd-103">Working with the communications API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd9fd-104">Microsoft Graph 通信 API 通过在应用和服务中启用核心通信功能，为你或你的组织与其他用户交互的方式添加了新的维度。</span><span class="sxs-lookup"><span data-stu-id="bd9fd-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="bd9fd-105">可使用此 API 接听电话、创建和检索会议坐标和查看用户的状态。</span><span class="sxs-lookup"><span data-stu-id="bd9fd-105">You can use this API to create and receive calls, create and retrieve meeting coordinates, and check users' presence.</span></span>

<span data-ttu-id="bd9fd-106">可使用通信 API 构建服务应用程序（机器人），它们在通话中充当参与者，代表用户创建和检索会议并检查出席状态和活动。</span><span class="sxs-lookup"><span data-stu-id="bd9fd-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users and to check their presence availability and activity.</span></span>
<span data-ttu-id="bd9fd-107">此 API 提供了通话功能，还可用于创建和检索联机会议。</span><span class="sxs-lookup"><span data-stu-id="bd9fd-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="bd9fd-108">可将服务应用程序（机器人）与此 API 搭配使用，其中机器人可在 VoIP 通话或 Microsoft Teams 会议中充当参与者等等。</span><span class="sxs-lookup"><span data-stu-id="bd9fd-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="bd9fd-109">授权</span><span class="sxs-lookup"><span data-stu-id="bd9fd-109">Authorization</span></span>

<span data-ttu-id="bd9fd-110">需要以下[权限](/graph/permissions-reference#calls-permissions) 之一才能访问通信 API。</span><span class="sxs-lookup"><span data-stu-id="bd9fd-110">One of the following [permissions](/graph/permissions-reference#calls-permissions) is required to access the communications API.</span></span> <span data-ttu-id="bd9fd-111">需要由管理员授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="bd9fd-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="bd9fd-112">方案</span><span class="sxs-lookup"><span data-stu-id="bd9fd-112">Scenario</span></span>                 | <span data-ttu-id="bd9fd-113">权限</span><span class="sxs-lookup"><span data-stu-id="bd9fd-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="bd9fd-114">通话</span><span class="sxs-lookup"><span data-stu-id="bd9fd-114">Calling</span></span>                 | <span data-ttu-id="bd9fd-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="bd9fd-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="bd9fd-116">会议</span><span class="sxs-lookup"><span data-stu-id="bd9fd-116">Meetings</span></span>                 | <span data-ttu-id="bd9fd-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd9fd-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |
| <span data-ttu-id="bd9fd-118">状态</span><span class="sxs-lookup"><span data-stu-id="bd9fd-118">Presence</span></span>                 | <span data-ttu-id="bd9fd-119">状态.阅读，状态.阅读.全部</span><span class="sxs-lookup"><span data-stu-id="bd9fd-119">Presence.Read, Presence.Read.All</span></span> |
| <span data-ttu-id="bd9fd-120">通话记录</span><span class="sxs-lookup"><span data-stu-id="bd9fd-120">Call records</span></span>             | <span data-ttu-id="bd9fd-121">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd9fd-121">CallRecords.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="bd9fd-122">常见用例</span><span class="sxs-lookup"><span data-stu-id="bd9fd-122">Common use cases</span></span>

<span data-ttu-id="bd9fd-123">下表列出了通信 API 的一些常见用例。</span><span class="sxs-lookup"><span data-stu-id="bd9fd-123">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="bd9fd-124">用例</span><span class="sxs-lookup"><span data-stu-id="bd9fd-124">Use cases</span></span>                         | <span data-ttu-id="bd9fd-125">REST 资源</span><span class="sxs-lookup"><span data-stu-id="bd9fd-125">REST resources</span></span>                                 | <span data-ttu-id="bd9fd-126">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bd9fd-126">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="bd9fd-127">创建并键入一对一通话和群组通话</span><span class="sxs-lookup"><span data-stu-id="bd9fd-127">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="bd9fd-128">通话</span><span class="sxs-lookup"><span data-stu-id="bd9fd-128">Call</span></span>](/graph/api/resources/call?view=graph-rest-beta)| [<span data-ttu-id="bd9fd-129">通话方法</span><span class="sxs-lookup"><span data-stu-id="bd9fd-129">Methods for calls</span></span>](/graph/api/resources/call?view=graph-rest-beta#methods)|
|<span data-ttu-id="bd9fd-130">IVR 通话</span><span class="sxs-lookup"><span data-stu-id="bd9fd-130">IVR calls</span></span>   |     | [<span data-ttu-id="bd9fd-131">IVR 方法</span><span class="sxs-lookup"><span data-stu-id="bd9fd-131">Methods for IVR</span></span>](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta)
| <span data-ttu-id="bd9fd-132">通话控制（参与者）</span><span class="sxs-lookup"><span data-stu-id="bd9fd-132">Call controls (participant)</span></span> | [<span data-ttu-id="bd9fd-133">参与者</span><span class="sxs-lookup"><span data-stu-id="bd9fd-133">Participant</span></span>](/graph/api/resources/participant?view=graph-rest-beta)   ||
|<span data-ttu-id="bd9fd-134">会议</span><span class="sxs-lookup"><span data-stu-id="bd9fd-134">Meetings</span></span>|[<span data-ttu-id="bd9fd-135">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="bd9fd-135">onlineMeeting</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-beta)| [<span data-ttu-id="bd9fd-136">会议方法</span><span class="sxs-lookup"><span data-stu-id="bd9fd-136">Methods for meetings</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-beta#methods)|
|<span data-ttu-id="bd9fd-137">状态</span><span class="sxs-lookup"><span data-stu-id="bd9fd-137">Presence</span></span> | [<span data-ttu-id="bd9fd-138">状态</span><span class="sxs-lookup"><span data-stu-id="bd9fd-138">presence</span></span>](/graph/api/resources/presence) | [<span data-ttu-id="bd9fd-139">出席方式</span><span class="sxs-lookup"><span data-stu-id="bd9fd-139">Methods for presence</span></span>](/graph/api/resources/presence#methods) |
| <span data-ttu-id="bd9fd-140">检索通话记录</span><span class="sxs-lookup"><span data-stu-id="bd9fd-140">Retrieving call records</span></span> | [<span data-ttu-id="bd9fd-141">callRecord</span><span class="sxs-lookup"><span data-stu-id="bd9fd-141">callRecord</span></span>](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta) | [<span data-ttu-id="bd9fd-142">Webhook 订阅</span><span class="sxs-lookup"><span data-stu-id="bd9fd-142">Webhook subscriptions</span></span>](/graph/api/resources/webhooks?view=graph-rest-beta) |

## <a name="common-properties"></a><span data-ttu-id="bd9fd-143">通用属性</span><span class="sxs-lookup"><span data-stu-id="bd9fd-143">Common properties</span></span>

| <span data-ttu-id="bd9fd-144">资源</span><span class="sxs-lookup"><span data-stu-id="bd9fd-144">Resource</span></span>                | <span data-ttu-id="bd9fd-145">属性</span><span class="sxs-lookup"><span data-stu-id="bd9fd-145">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="bd9fd-146">通话</span><span class="sxs-lookup"><span data-stu-id="bd9fd-146">call</span></span>                               | [<span data-ttu-id="bd9fd-147">通话属性</span><span class="sxs-lookup"><span data-stu-id="bd9fd-147">call properties</span></span>](/graph/api/resources/call?view=graph-rest-beta#properties)  |
| <span data-ttu-id="bd9fd-148">参与者</span><span class="sxs-lookup"><span data-stu-id="bd9fd-148">participant</span></span>                         | [<span data-ttu-id="bd9fd-149">参与者属性</span><span class="sxs-lookup"><span data-stu-id="bd9fd-149">participant properties</span></span>](/graph/api/resources/participant?view=graph-rest-beta#properties) |
| <span data-ttu-id="bd9fd-150">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="bd9fd-150">onlineMeeting</span></span>                            | [<span data-ttu-id="bd9fd-151">onlineMeeting 属性</span><span class="sxs-lookup"><span data-stu-id="bd9fd-151">onlineMeeting properties</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-beta#properties)                     |
| <span data-ttu-id="bd9fd-152">状态</span><span class="sxs-lookup"><span data-stu-id="bd9fd-152">presence</span></span> | [<span data-ttu-id="bd9fd-153">状态属性</span><span class="sxs-lookup"><span data-stu-id="bd9fd-153">presence properties</span></span>](/graph/api/resources/presence#properties) |
| <span data-ttu-id="bd9fd-154">callRecord</span><span class="sxs-lookup"><span data-stu-id="bd9fd-154">callRecord</span></span> | [<span data-ttu-id="bd9fd-155">callRecord 属性</span><span class="sxs-lookup"><span data-stu-id="bd9fd-155">callRecord properties</span></span>](/graph/api/resources/callrecords-callrecord#properties) |

## <a name="whats-new"></a><span data-ttu-id="bd9fd-156">最近更新</span><span class="sxs-lookup"><span data-stu-id="bd9fd-156">What's new</span></span>
<span data-ttu-id="bd9fd-157">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="bd9fd-157">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="see-also"></a><span data-ttu-id="bd9fd-158">另请参阅</span><span class="sxs-lookup"><span data-stu-id="bd9fd-158">See also</span></span>

- [<span data-ttu-id="bd9fd-159">通信 API 示例</span><span class="sxs-lookup"><span data-stu-id="bd9fd-159">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="bd9fd-160">通信信号 SDK</span><span class="sxs-lookup"><span data-stu-id="bd9fd-160">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls/1.0.0-prerelease.494)
- [<span data-ttu-id="bd9fd-161">通信媒体 SDK</span><span class="sxs-lookup"><span data-stu-id="bd9fd-161">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media/1.0.0-prerelease.494)
