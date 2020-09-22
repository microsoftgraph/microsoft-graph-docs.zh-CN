---
title: 使用 Microsoft Graph 通信 API
description: Microsoft Graph 通信 API 通过启用语音和视频功能，为应用和服务与用户的互动方式添加了新的维度。
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 5cdd723e9d73a0466ae4349026f6bf086cb9bdd2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091864"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="acff2-103">使用 Microsoft Graph 通信 API</span><span class="sxs-lookup"><span data-stu-id="acff2-103">Working with the communications API in Microsoft Graph</span></span>

<span data-ttu-id="acff2-104">Microsoft Graph 通信 API 通过在应用和服务中启用核心通信功能，为你或你的组织与其他用户交互的方式添加了新的维度。</span><span class="sxs-lookup"><span data-stu-id="acff2-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="acff2-105">可使用此 API 接听电话、创建和检索会议坐标。</span><span class="sxs-lookup"><span data-stu-id="acff2-105">You can use this API to create and receive calls as well as create and retrieve meeting coordinates.</span></span>

<span data-ttu-id="acff2-106">可使用通信 API 构建服务应用程序（机器人），它们在通话中充当参与者，并代表用户创建和检索会议。</span><span class="sxs-lookup"><span data-stu-id="acff2-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users.</span></span>
<span data-ttu-id="acff2-107">此 API 提供了通话功能，还可用于创建和检索联机会议。</span><span class="sxs-lookup"><span data-stu-id="acff2-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="acff2-108">可将服务应用程序（机器人）与此 API 搭配使用，其中机器人可在 VoIP 通话或 Microsoft Teams 会议中充当参与者等等。</span><span class="sxs-lookup"><span data-stu-id="acff2-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="acff2-109">授权</span><span class="sxs-lookup"><span data-stu-id="acff2-109">Authorization</span></span>

<span data-ttu-id="acff2-110">需要以下[权限](https://docs.microsoft.com/graph/permissions-reference#calls-permissions) 之一才能访问通信 API。</span><span class="sxs-lookup"><span data-stu-id="acff2-110">One of the following [permissions](https://docs.microsoft.com/graph/permissions-reference#calls-permissions) is required to access the communications API.</span></span> <span data-ttu-id="acff2-111">需要由管理员授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="acff2-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="acff2-112">方案</span><span class="sxs-lookup"><span data-stu-id="acff2-112">Scenario</span></span>                 | <span data-ttu-id="acff2-113">权限</span><span class="sxs-lookup"><span data-stu-id="acff2-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="acff2-114">通话</span><span class="sxs-lookup"><span data-stu-id="acff2-114">Calling</span></span>                 | <span data-ttu-id="acff2-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="acff2-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="acff2-116">会议</span><span class="sxs-lookup"><span data-stu-id="acff2-116">Meetings</span></span>                 | <span data-ttu-id="acff2-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="acff2-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |
| <span data-ttu-id="acff2-118">通话记录</span><span class="sxs-lookup"><span data-stu-id="acff2-118">Call records</span></span>             | <span data-ttu-id="acff2-119">CallRecords.Read.All</span><span class="sxs-lookup"><span data-stu-id="acff2-119">CallRecords.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="acff2-120">常见用例</span><span class="sxs-lookup"><span data-stu-id="acff2-120">Common use cases</span></span>

<span data-ttu-id="acff2-121">下表列出了通信 API 的一些常见用例。</span><span class="sxs-lookup"><span data-stu-id="acff2-121">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="acff2-122">用例</span><span class="sxs-lookup"><span data-stu-id="acff2-122">Use cases</span></span>                         | <span data-ttu-id="acff2-123">REST 资源</span><span class="sxs-lookup"><span data-stu-id="acff2-123">REST resources</span></span>                                 | <span data-ttu-id="acff2-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="acff2-124">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="acff2-125">创建并键入一对一通话和群组通话</span><span class="sxs-lookup"><span data-stu-id="acff2-125">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="acff2-126">通话</span><span class="sxs-lookup"><span data-stu-id="acff2-126">Call</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0)| [<span data-ttu-id="acff2-127">通话方法</span><span class="sxs-lookup"><span data-stu-id="acff2-127">Methods for calls</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#methods)| 
|<span data-ttu-id="acff2-128">IVR 通话</span><span class="sxs-lookup"><span data-stu-id="acff2-128">IVR calls</span></span>   |     | [<span data-ttu-id="acff2-129">IVR 方法</span><span class="sxs-lookup"><span data-stu-id="acff2-129">Methods for IVR</span></span>](https://docs.microsoft.com/graph/api/resources/calls-api-ivr-overview?view=graph-rest-v1.0)
| <span data-ttu-id="acff2-130">通话控制（参与者）</span><span class="sxs-lookup"><span data-stu-id="acff2-130">Call controls (participant)</span></span> | [<span data-ttu-id="acff2-131">参与者</span><span class="sxs-lookup"><span data-stu-id="acff2-131">Participant</span></span>](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0)   ||
|<span data-ttu-id="acff2-132">会议</span><span class="sxs-lookup"><span data-stu-id="acff2-132">Meetings</span></span>|[<span data-ttu-id="acff2-133">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="acff2-133">onlineMeeting</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0)| [<span data-ttu-id="acff2-134">会议方法</span><span class="sxs-lookup"><span data-stu-id="acff2-134">Methods for meetings</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#methods)|
| <span data-ttu-id="acff2-135">检索通话记录</span><span class="sxs-lookup"><span data-stu-id="acff2-135">Retrieving call records</span></span> | [<span data-ttu-id="acff2-136">callRecord</span><span class="sxs-lookup"><span data-stu-id="acff2-136">callRecord</span></span>](/graph/api/resources/callrecords-callrecord?view=graph-rest-1.0) | [<span data-ttu-id="acff2-137">Webhook 订阅</span><span class="sxs-lookup"><span data-stu-id="acff2-137">Webhook subscriptions</span></span>](/graph/api/resources/webhooks?view=graph-rest-1.0) |

## <a name="common-properties"></a><span data-ttu-id="acff2-138">通用属性</span><span class="sxs-lookup"><span data-stu-id="acff2-138">Common properties</span></span>

| <span data-ttu-id="acff2-139">资源</span><span class="sxs-lookup"><span data-stu-id="acff2-139">Resource</span></span>                | <span data-ttu-id="acff2-140">属性</span><span class="sxs-lookup"><span data-stu-id="acff2-140">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="acff2-141">通话</span><span class="sxs-lookup"><span data-stu-id="acff2-141">call</span></span>                               | [<span data-ttu-id="acff2-142">通话属性</span><span class="sxs-lookup"><span data-stu-id="acff2-142">call properties</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#properties)  |
| <span data-ttu-id="acff2-143">参与者</span><span class="sxs-lookup"><span data-stu-id="acff2-143">participant</span></span>                         | [<span data-ttu-id="acff2-144">参与者属性</span><span class="sxs-lookup"><span data-stu-id="acff2-144">participant properties</span></span>](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0#properties) |
| <span data-ttu-id="acff2-145">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="acff2-145">onlineMeeting</span></span>                            | [<span data-ttu-id="acff2-146">onlineMeeting 属性</span><span class="sxs-lookup"><span data-stu-id="acff2-146">onlineMeeting properties</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#properties)                     |
| <span data-ttu-id="acff2-147">callRecord</span><span class="sxs-lookup"><span data-stu-id="acff2-147">callRecord</span></span> | [<span data-ttu-id="acff2-148">callRecord 属性</span><span class="sxs-lookup"><span data-stu-id="acff2-148">callRecord properties</span></span>](/graph/api/resources/callrecords-callrecord#properties) |

## <a name="whats-new"></a><span data-ttu-id="acff2-149">最近更新</span><span class="sxs-lookup"><span data-stu-id="acff2-149">What's new</span></span>
<span data-ttu-id="acff2-150">了解此 API 集的[最新功能和更新](/graph/whats-new-overview)。</span><span class="sxs-lookup"><span data-stu-id="acff2-150">Find out about the [latest new features and updates](/graph/whats-new-overview) for this API set.</span></span>

## <a name="see-also"></a><span data-ttu-id="acff2-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="acff2-151">See also</span></span>

- [<span data-ttu-id="acff2-152">通信 API 示例</span><span class="sxs-lookup"><span data-stu-id="acff2-152">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="acff2-153">通信信号 SDK</span><span class="sxs-lookup"><span data-stu-id="acff2-153">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)
- [<span data-ttu-id="acff2-154">通信媒体 SDK</span><span class="sxs-lookup"><span data-stu-id="acff2-154">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media)

