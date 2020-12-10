---
title: 使用 Microsoft Graph 通信 API
description: Microsoft Graph 通信 API 通过启用语音和视频功能，为应用和服务与用户的互动方式添加了新的维度。
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: e6e6c4ba8d262ac01846b6ed06938b2c5c89350b
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581136"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="4a1f1-103">使用 Microsoft Graph 通信 API</span><span class="sxs-lookup"><span data-stu-id="4a1f1-103">Working with the communications API in Microsoft Graph</span></span>

<span data-ttu-id="4a1f1-104">Microsoft Graph 通信 API 通过在应用和服务中启用核心通信功能，为你或你的组织与其他用户交互的方式添加了新的维度。</span><span class="sxs-lookup"><span data-stu-id="4a1f1-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="4a1f1-105">可使用此 API 接听电话、创建和检索会议坐标。</span><span class="sxs-lookup"><span data-stu-id="4a1f1-105">You can use this API to create and receive calls as well as create and retrieve meeting coordinates.</span></span>

<span data-ttu-id="4a1f1-106">可使用通信 API 构建服务应用程序（机器人），它们在通话中充当参与者，并代表用户创建和检索会议。</span><span class="sxs-lookup"><span data-stu-id="4a1f1-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users.</span></span>
<span data-ttu-id="4a1f1-107">此 API 提供了通话功能，还可用于创建和检索联机会议。</span><span class="sxs-lookup"><span data-stu-id="4a1f1-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="4a1f1-108">可将服务应用程序（机器人）与此 API 搭配使用，其中机器人可在 VoIP 通话或 Microsoft Teams 会议中充当参与者等等。</span><span class="sxs-lookup"><span data-stu-id="4a1f1-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="4a1f1-109">授权</span><span class="sxs-lookup"><span data-stu-id="4a1f1-109">Authorization</span></span>

<span data-ttu-id="4a1f1-110">需要以下[权限](/graph/permissions-reference#calls-permissions) 之一才能访问通信 API。</span><span class="sxs-lookup"><span data-stu-id="4a1f1-110">One of the following [permissions](/graph/permissions-reference#calls-permissions) is required to access the communications API.</span></span> <span data-ttu-id="4a1f1-111">需要由管理员授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="4a1f1-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="4a1f1-112">方案</span><span class="sxs-lookup"><span data-stu-id="4a1f1-112">Scenario</span></span>                 | <span data-ttu-id="4a1f1-113">权限</span><span class="sxs-lookup"><span data-stu-id="4a1f1-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="4a1f1-114">通话</span><span class="sxs-lookup"><span data-stu-id="4a1f1-114">Calling</span></span>                 | <span data-ttu-id="4a1f1-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="4a1f1-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="4a1f1-116">会议</span><span class="sxs-lookup"><span data-stu-id="4a1f1-116">Meetings</span></span>                 | <span data-ttu-id="4a1f1-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a1f1-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |
| <span data-ttu-id="4a1f1-118">通话记录</span><span class="sxs-lookup"><span data-stu-id="4a1f1-118">Call records</span></span>             | <span data-ttu-id="4a1f1-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="4a1f1-119">CallRecords.Read.All</span></span> |
| <span data-ttu-id="4a1f1-120">状态</span><span class="sxs-lookup"><span data-stu-id="4a1f1-120">Presences</span></span>             | <span data-ttu-id="4a1f1-121">状态.阅读，状态.阅读.全部</span><span class="sxs-lookup"><span data-stu-id="4a1f1-121">Presence.Read, Presence.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="4a1f1-122">常见用例</span><span class="sxs-lookup"><span data-stu-id="4a1f1-122">Common use cases</span></span>

<span data-ttu-id="4a1f1-123">下表列出了通信 API 的一些常见用例。</span><span class="sxs-lookup"><span data-stu-id="4a1f1-123">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="4a1f1-124">用例</span><span class="sxs-lookup"><span data-stu-id="4a1f1-124">Use cases</span></span>                         | <span data-ttu-id="4a1f1-125">REST 资源</span><span class="sxs-lookup"><span data-stu-id="4a1f1-125">REST resources</span></span>                                 | <span data-ttu-id="4a1f1-126">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4a1f1-126">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="4a1f1-127">创建并键入一对一通话和群组通话</span><span class="sxs-lookup"><span data-stu-id="4a1f1-127">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="4a1f1-128">通话</span><span class="sxs-lookup"><span data-stu-id="4a1f1-128">Call</span></span>](/graph/api/resources/call?view=graph-rest-v1.0)| [<span data-ttu-id="4a1f1-129">通话方法</span><span class="sxs-lookup"><span data-stu-id="4a1f1-129">Methods for calls</span></span>](/graph/api/resources/call?view=graph-rest-v1.0#methods)| 
|<span data-ttu-id="4a1f1-130">IVR 通话</span><span class="sxs-lookup"><span data-stu-id="4a1f1-130">IVR calls</span></span>   |     | [<span data-ttu-id="4a1f1-131">IVR 方法</span><span class="sxs-lookup"><span data-stu-id="4a1f1-131">Methods for IVR</span></span>](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-v1.0)
| <span data-ttu-id="4a1f1-132">通话控制（参与者）</span><span class="sxs-lookup"><span data-stu-id="4a1f1-132">Call controls (participant)</span></span> | [<span data-ttu-id="4a1f1-133">参与者</span><span class="sxs-lookup"><span data-stu-id="4a1f1-133">Participant</span></span>](/graph/api/resources/participant?view=graph-rest-v1.0)   ||
|<span data-ttu-id="4a1f1-134">会议</span><span class="sxs-lookup"><span data-stu-id="4a1f1-134">Meetings</span></span>|[<span data-ttu-id="4a1f1-135">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="4a1f1-135">onlineMeeting</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-v1.0)| [<span data-ttu-id="4a1f1-136">会议方法</span><span class="sxs-lookup"><span data-stu-id="4a1f1-136">Methods for meetings</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#methods)|
| <span data-ttu-id="4a1f1-137">检索通话记录</span><span class="sxs-lookup"><span data-stu-id="4a1f1-137">Retrieving call records</span></span> | [<span data-ttu-id="4a1f1-138">callRecord</span><span class="sxs-lookup"><span data-stu-id="4a1f1-138">callRecord</span></span>](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) | [<span data-ttu-id="4a1f1-139">Webhook 订阅</span><span class="sxs-lookup"><span data-stu-id="4a1f1-139">Webhook subscriptions</span></span>](/graph/api/resources/webhooks?view=graph-rest-1.0) |
|<span data-ttu-id="4a1f1-140">状态</span><span class="sxs-lookup"><span data-stu-id="4a1f1-140">Presences</span></span>|[<span data-ttu-id="4a1f1-141">状态</span><span class="sxs-lookup"><span data-stu-id="4a1f1-141">presence</span></span>](/graph/api/resources/presence?view=graph-rest-v1.0)||

## <a name="common-properties"></a><span data-ttu-id="4a1f1-142">通用属性</span><span class="sxs-lookup"><span data-stu-id="4a1f1-142">Common properties</span></span>

| <span data-ttu-id="4a1f1-143">资源</span><span class="sxs-lookup"><span data-stu-id="4a1f1-143">Resource</span></span>                | <span data-ttu-id="4a1f1-144">属性</span><span class="sxs-lookup"><span data-stu-id="4a1f1-144">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="4a1f1-145">通话</span><span class="sxs-lookup"><span data-stu-id="4a1f1-145">call</span></span>                               | [<span data-ttu-id="4a1f1-146">通话属性</span><span class="sxs-lookup"><span data-stu-id="4a1f1-146">call properties</span></span>](/graph/api/resources/call?view=graph-rest-v1.0#properties)  |
| <span data-ttu-id="4a1f1-147">参与者</span><span class="sxs-lookup"><span data-stu-id="4a1f1-147">participant</span></span>                         | [<span data-ttu-id="4a1f1-148">参与者属性</span><span class="sxs-lookup"><span data-stu-id="4a1f1-148">participant properties</span></span>](/graph/api/resources/participant?view=graph-rest-v1.0#properties) |
| <span data-ttu-id="4a1f1-149">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="4a1f1-149">onlineMeeting</span></span>                            | [<span data-ttu-id="4a1f1-150">onlineMeeting 属性</span><span class="sxs-lookup"><span data-stu-id="4a1f1-150">onlineMeeting properties</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#properties)                     |
| <span data-ttu-id="4a1f1-151">callRecord</span><span class="sxs-lookup"><span data-stu-id="4a1f1-151">callRecord</span></span> | [<span data-ttu-id="4a1f1-152">callRecord 属性</span><span class="sxs-lookup"><span data-stu-id="4a1f1-152">callRecord properties</span></span>](/graph/api/resources/callrecords-callrecord#properties) |
|<span data-ttu-id="4a1f1-153">状态</span><span class="sxs-lookup"><span data-stu-id="4a1f1-153">presence</span></span>|[<span data-ttu-id="4a1f1-154">状态</span><span class="sxs-lookup"><span data-stu-id="4a1f1-154">presence</span></span>](/graph/api/resources/presence?view=graph-rest-v1.0)|

## <a name="whats-new"></a><span data-ttu-id="4a1f1-155">最近更新</span><span class="sxs-lookup"><span data-stu-id="4a1f1-155">What's new</span></span>
<span data-ttu-id="4a1f1-156">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="4a1f1-156">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="see-also"></a><span data-ttu-id="4a1f1-157">另请参阅</span><span class="sxs-lookup"><span data-stu-id="4a1f1-157">See also</span></span>

- [<span data-ttu-id="4a1f1-158">通信 API 示例</span><span class="sxs-lookup"><span data-stu-id="4a1f1-158">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="4a1f1-159">通信信号 SDK</span><span class="sxs-lookup"><span data-stu-id="4a1f1-159">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)
- [<span data-ttu-id="4a1f1-160">通信媒体 SDK</span><span class="sxs-lookup"><span data-stu-id="4a1f1-160">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media)