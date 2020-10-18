---
title: 使用 Microsoft Graph 通信 API
description: Microsoft Graph 通信 API 通过启用语音和视频功能，为应用和服务与用户的互动方式添加了新的维度。
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: ef67a53cb38f0a146069005c45297972298f4b85
ms.sourcegitcommit: 577bfd3bb8a2e2679ef1c5942a4a496c2aa3a277
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/17/2020
ms.locfileid: "48582329"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="d31b4-103">使用 Microsoft Graph 通信 API</span><span class="sxs-lookup"><span data-stu-id="d31b4-103">Working with the communications API in Microsoft Graph</span></span>

<span data-ttu-id="d31b4-104">Microsoft Graph 通信 API 通过在应用和服务中启用核心通信功能，为你或你的组织与其他用户交互的方式添加了新的维度。</span><span class="sxs-lookup"><span data-stu-id="d31b4-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="d31b4-105">可使用此 API 接听电话、创建和检索会议坐标。</span><span class="sxs-lookup"><span data-stu-id="d31b4-105">You can use this API to create and receive calls as well as create and retrieve meeting coordinates.</span></span>

<span data-ttu-id="d31b4-106">可使用通信 API 构建服务应用程序（机器人），它们在通话中充当参与者，并代表用户创建和检索会议。</span><span class="sxs-lookup"><span data-stu-id="d31b4-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users.</span></span>
<span data-ttu-id="d31b4-107">此 API 提供了通话功能，还可用于创建和检索联机会议。</span><span class="sxs-lookup"><span data-stu-id="d31b4-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="d31b4-108">可将服务应用程序（机器人）与此 API 搭配使用，其中机器人可在 VoIP 通话或 Microsoft Teams 会议中充当参与者等等。</span><span class="sxs-lookup"><span data-stu-id="d31b4-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="d31b4-109">授权</span><span class="sxs-lookup"><span data-stu-id="d31b4-109">Authorization</span></span>

<span data-ttu-id="d31b4-110">需要以下[权限](/graph/permissions-reference#calls-permissions) 之一才能访问通信 API。</span><span class="sxs-lookup"><span data-stu-id="d31b4-110">One of the following [permissions](/graph/permissions-reference#calls-permissions) is required to access the communications API.</span></span> <span data-ttu-id="d31b4-111">需要由管理员授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="d31b4-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="d31b4-112">方案</span><span class="sxs-lookup"><span data-stu-id="d31b4-112">Scenario</span></span>                 | <span data-ttu-id="d31b4-113">权限</span><span class="sxs-lookup"><span data-stu-id="d31b4-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="d31b4-114">通话</span><span class="sxs-lookup"><span data-stu-id="d31b4-114">Calling</span></span>                 | <span data-ttu-id="d31b4-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="d31b4-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="d31b4-116">会议</span><span class="sxs-lookup"><span data-stu-id="d31b4-116">Meetings</span></span>                 | <span data-ttu-id="d31b4-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="d31b4-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |
| <span data-ttu-id="d31b4-118">通话记录</span><span class="sxs-lookup"><span data-stu-id="d31b4-118">Call records</span></span>             | <span data-ttu-id="d31b4-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="d31b4-119">CallRecords.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="d31b4-120">常见用例</span><span class="sxs-lookup"><span data-stu-id="d31b4-120">Common use cases</span></span>

<span data-ttu-id="d31b4-121">下表列出了通信 API 的一些常见用例。</span><span class="sxs-lookup"><span data-stu-id="d31b4-121">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="d31b4-122">用例</span><span class="sxs-lookup"><span data-stu-id="d31b4-122">Use cases</span></span>                         | <span data-ttu-id="d31b4-123">REST 资源</span><span class="sxs-lookup"><span data-stu-id="d31b4-123">REST resources</span></span>                                 | <span data-ttu-id="d31b4-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d31b4-124">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="d31b4-125">创建并键入一对一通话和群组通话</span><span class="sxs-lookup"><span data-stu-id="d31b4-125">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="d31b4-126">通话</span><span class="sxs-lookup"><span data-stu-id="d31b4-126">Call</span></span>](/graph/api/resources/call?view=graph-rest-v1.0)| [<span data-ttu-id="d31b4-127">通话方法</span><span class="sxs-lookup"><span data-stu-id="d31b4-127">Methods for calls</span></span>](/graph/api/resources/call?view=graph-rest-v1.0#methods)| 
|<span data-ttu-id="d31b4-128">IVR 通话</span><span class="sxs-lookup"><span data-stu-id="d31b4-128">IVR calls</span></span>   |     | [<span data-ttu-id="d31b4-129">IVR 方法</span><span class="sxs-lookup"><span data-stu-id="d31b4-129">Methods for IVR</span></span>](/graph/api/resources/calls-api-ivr-overview?view=graph-rest-v1.0)
| <span data-ttu-id="d31b4-130">通话控制（参与者）</span><span class="sxs-lookup"><span data-stu-id="d31b4-130">Call controls (participant)</span></span> | [<span data-ttu-id="d31b4-131">参与者</span><span class="sxs-lookup"><span data-stu-id="d31b4-131">Participant</span></span>](/graph/api/resources/participant?view=graph-rest-v1.0)   ||
|<span data-ttu-id="d31b4-132">会议</span><span class="sxs-lookup"><span data-stu-id="d31b4-132">Meetings</span></span>|[<span data-ttu-id="d31b4-133">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="d31b4-133">onlineMeeting</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-v1.0)| [<span data-ttu-id="d31b4-134">会议方法</span><span class="sxs-lookup"><span data-stu-id="d31b4-134">Methods for meetings</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#methods)|
| <span data-ttu-id="d31b4-135">检索通话记录</span><span class="sxs-lookup"><span data-stu-id="d31b4-135">Retrieving call records</span></span> | [<span data-ttu-id="d31b4-136">callRecord</span><span class="sxs-lookup"><span data-stu-id="d31b4-136">callRecord</span></span>](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) | [<span data-ttu-id="d31b4-137">Webhook 订阅</span><span class="sxs-lookup"><span data-stu-id="d31b4-137">Webhook subscriptions</span></span>](/graph/api/resources/webhooks?view=graph-rest-1.0) |

## <a name="common-properties"></a><span data-ttu-id="d31b4-138">通用属性</span><span class="sxs-lookup"><span data-stu-id="d31b4-138">Common properties</span></span>

| <span data-ttu-id="d31b4-139">资源</span><span class="sxs-lookup"><span data-stu-id="d31b4-139">Resource</span></span>                | <span data-ttu-id="d31b4-140">属性</span><span class="sxs-lookup"><span data-stu-id="d31b4-140">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="d31b4-141">通话</span><span class="sxs-lookup"><span data-stu-id="d31b4-141">call</span></span>                               | [<span data-ttu-id="d31b4-142">通话属性</span><span class="sxs-lookup"><span data-stu-id="d31b4-142">call properties</span></span>](/graph/api/resources/call?view=graph-rest-v1.0#properties)  |
| <span data-ttu-id="d31b4-143">参与者</span><span class="sxs-lookup"><span data-stu-id="d31b4-143">participant</span></span>                         | [<span data-ttu-id="d31b4-144">参与者属性</span><span class="sxs-lookup"><span data-stu-id="d31b4-144">participant properties</span></span>](/graph/api/resources/participant?view=graph-rest-v1.0#properties) |
| <span data-ttu-id="d31b4-145">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="d31b4-145">onlineMeeting</span></span>                            | [<span data-ttu-id="d31b4-146">onlineMeeting 属性</span><span class="sxs-lookup"><span data-stu-id="d31b4-146">onlineMeeting properties</span></span>](/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#properties)                     |
| <span data-ttu-id="d31b4-147">callRecord</span><span class="sxs-lookup"><span data-stu-id="d31b4-147">callRecord</span></span> | [<span data-ttu-id="d31b4-148">callRecord 属性</span><span class="sxs-lookup"><span data-stu-id="d31b4-148">callRecord properties</span></span>](/graph/api/resources/callrecords-callrecord#properties) |

## <a name="whats-new"></a><span data-ttu-id="d31b4-149">最近更新</span><span class="sxs-lookup"><span data-stu-id="d31b4-149">What's new</span></span>
<span data-ttu-id="d31b4-150">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="d31b4-150">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="see-also"></a><span data-ttu-id="d31b4-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="d31b4-151">See also</span></span>

- [<span data-ttu-id="d31b4-152">通信 API 示例</span><span class="sxs-lookup"><span data-stu-id="d31b4-152">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="d31b4-153">通信信号 SDK</span><span class="sxs-lookup"><span data-stu-id="d31b4-153">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)
- [<span data-ttu-id="d31b4-154">通信媒体 SDK</span><span class="sxs-lookup"><span data-stu-id="d31b4-154">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media)