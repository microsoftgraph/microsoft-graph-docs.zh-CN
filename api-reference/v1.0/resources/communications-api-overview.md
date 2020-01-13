---
title: 使用 Microsoft Graph 通信 API
description: Microsoft Graph 通信 API 通过启用语音和视频功能，为应用和服务与用户的互动方式添加了新的维度。
author: ananmishr
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: b17dc07431bfe579125d162754c4f4ad4110e73f
ms.sourcegitcommit: 2a601cffdb8df375b2ee32a1f35b8f71e0ffd04f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2020
ms.locfileid: "41023073"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="6d85a-103">使用 Microsoft Graph 通信 API</span><span class="sxs-lookup"><span data-stu-id="6d85a-103">Working with the communications API in Microsoft Graph</span></span>

<span data-ttu-id="6d85a-104">Microsoft Graph 通信 API 通过在应用和服务中启用核心通信功能，为你或你的组织与其他用户交互的方式添加了新的维度。</span><span class="sxs-lookup"><span data-stu-id="6d85a-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="6d85a-105">可使用此 API 接听电话、创建和检索会议坐标。</span><span class="sxs-lookup"><span data-stu-id="6d85a-105">You can use this API to create and receive calls as well as create and retrieve meeting coordinates.</span></span>

<span data-ttu-id="6d85a-106">可使用通信 API 构建服务应用程序（机器人），它们在通话中充当参与者，并代表用户创建和检索会议。</span><span class="sxs-lookup"><span data-stu-id="6d85a-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users.</span></span>
<span data-ttu-id="6d85a-107">此 API 提供了通话功能，还可用于创建和检索联机会议。</span><span class="sxs-lookup"><span data-stu-id="6d85a-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="6d85a-108">可将服务应用程序（机器人）与此 API 搭配使用，其中机器人可在 VoIP 通话或 Microsoft Teams 会议中充当参与者等等。</span><span class="sxs-lookup"><span data-stu-id="6d85a-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="6d85a-109">授权</span><span class="sxs-lookup"><span data-stu-id="6d85a-109">Authorization</span></span>

<span data-ttu-id="6d85a-110">需要以下[权限](https://docs.microsoft.com/graph/permissions-reference#calls-permissions) 之一才能访问通信 API。</span><span class="sxs-lookup"><span data-stu-id="6d85a-110">One of the following [permissions](https://docs.microsoft.com/graph/permissions-reference#calls-permissions) is required to access the communications API.</span></span> <span data-ttu-id="6d85a-111">需要由管理员授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="6d85a-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="6d85a-112">方案</span><span class="sxs-lookup"><span data-stu-id="6d85a-112">Scenario</span></span>                 | <span data-ttu-id="6d85a-113">权限</span><span class="sxs-lookup"><span data-stu-id="6d85a-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="6d85a-114">通话</span><span class="sxs-lookup"><span data-stu-id="6d85a-114">Calling</span></span>                 | <span data-ttu-id="6d85a-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="6d85a-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="6d85a-116">会议</span><span class="sxs-lookup"><span data-stu-id="6d85a-116">Meetings</span></span>                 | <span data-ttu-id="6d85a-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="6d85a-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="6d85a-118">常见用例</span><span class="sxs-lookup"><span data-stu-id="6d85a-118">Common use cases</span></span>

<span data-ttu-id="6d85a-119">下表列出了通信 API 的一些常见用例。</span><span class="sxs-lookup"><span data-stu-id="6d85a-119">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="6d85a-120">用例</span><span class="sxs-lookup"><span data-stu-id="6d85a-120">Use cases</span></span>                         | <span data-ttu-id="6d85a-121">REST 资源</span><span class="sxs-lookup"><span data-stu-id="6d85a-121">REST resources</span></span>                                 | <span data-ttu-id="6d85a-122">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6d85a-122">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="6d85a-123">创建并键入一对一通话和群组通话</span><span class="sxs-lookup"><span data-stu-id="6d85a-123">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="6d85a-124">通话</span><span class="sxs-lookup"><span data-stu-id="6d85a-124">Call</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0)| [<span data-ttu-id="6d85a-125">通话方法</span><span class="sxs-lookup"><span data-stu-id="6d85a-125">Methods for calls</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#methods)| 
|<span data-ttu-id="6d85a-126">IVR 通话</span><span class="sxs-lookup"><span data-stu-id="6d85a-126">IVR calls</span></span>   |     | [<span data-ttu-id="6d85a-127">IVR 方法</span><span class="sxs-lookup"><span data-stu-id="6d85a-127">Methods for IVR</span></span>](https://docs.microsoft.com/graph/api/resources/calls-api-ivr-overview?view=graph-rest-v1.0)
| <span data-ttu-id="6d85a-128">通话控制（参与者）</span><span class="sxs-lookup"><span data-stu-id="6d85a-128">Call controls (participant)</span></span> | [<span data-ttu-id="6d85a-129">参与者</span><span class="sxs-lookup"><span data-stu-id="6d85a-129">Participant</span></span>](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0)   ||
|<span data-ttu-id="6d85a-130">会议</span><span class="sxs-lookup"><span data-stu-id="6d85a-130">Meetings</span></span>|[<span data-ttu-id="6d85a-131">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6d85a-131">onlineMeeting</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0)| [<span data-ttu-id="6d85a-132">会议方法</span><span class="sxs-lookup"><span data-stu-id="6d85a-132">Methods for meetings</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#methods)|

## <a name="common-properties"></a><span data-ttu-id="6d85a-133">通用属性</span><span class="sxs-lookup"><span data-stu-id="6d85a-133">Common properties</span></span>

| <span data-ttu-id="6d85a-134">资源</span><span class="sxs-lookup"><span data-stu-id="6d85a-134">Resource</span></span>                | <span data-ttu-id="6d85a-135">属性</span><span class="sxs-lookup"><span data-stu-id="6d85a-135">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="6d85a-136">通话</span><span class="sxs-lookup"><span data-stu-id="6d85a-136">call</span></span>                               | [<span data-ttu-id="6d85a-137">通话属性</span><span class="sxs-lookup"><span data-stu-id="6d85a-137">call properties</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-v1.0#properties)  |
| <span data-ttu-id="6d85a-138">参与者</span><span class="sxs-lookup"><span data-stu-id="6d85a-138">participant</span></span>                         | [<span data-ttu-id="6d85a-139">参与者属性</span><span class="sxs-lookup"><span data-stu-id="6d85a-139">participant properties</span></span>](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-v1.0#properties) |
| <span data-ttu-id="6d85a-140">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="6d85a-140">onlineMeeting</span></span>                            | [<span data-ttu-id="6d85a-141">onlineMeeting 属性</span><span class="sxs-lookup"><span data-stu-id="6d85a-141">onlineMeeting properties</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-v1.0#properties)                     |

## <a name="see-also"></a><span data-ttu-id="6d85a-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6d85a-142">See also</span></span>

- [<span data-ttu-id="6d85a-143">通信 API 示例</span><span class="sxs-lookup"><span data-stu-id="6d85a-143">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="6d85a-144">通信信号 SDK</span><span class="sxs-lookup"><span data-stu-id="6d85a-144">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls)
- [<span data-ttu-id="6d85a-145">通信媒体 SDK</span><span class="sxs-lookup"><span data-stu-id="6d85a-145">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media)
