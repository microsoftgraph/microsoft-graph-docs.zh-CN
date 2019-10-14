---
title: 使用 Microsoft Graph 通信 API
description: Microsoft Graph 通信 API 通过启用语音和视频功能，为应用和服务与用户的互动方式添加了新的维度。
author: VinodRavichandran
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: d5bcd46cb89a5d911c9286ef5c2093460949a3a1
ms.sourcegitcommit: 99cbeac2ca652632d2946c4740133c9b82c8e992
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/12/2019
ms.locfileid: "37477074"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="7238e-103">使用 Microsoft Graph 通信 API</span><span class="sxs-lookup"><span data-stu-id="7238e-103">Working with the calls and online meetings API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7238e-104">Microsoft Graph 通信 API 通过在应用和服务中启用核心通信功能，为你或你的组织与其他用户交互的方式添加了新的维度。</span><span class="sxs-lookup"><span data-stu-id="7238e-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="7238e-105">可使用此 API 接听电话、创建和检索会议坐标和查看用户的状态。</span><span class="sxs-lookup"><span data-stu-id="7238e-105">You can use this API to create and receive calls, create and retrieve meeting coordinates, and check users' presence.</span></span>

<span data-ttu-id="7238e-106">可使用通信 API 构建服务应用程序（机器人），它们在通话中充当参与者，并代表用户创建和检索会议。</span><span class="sxs-lookup"><span data-stu-id="7238e-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users.</span></span> <!-- and to check presence availability and activity of users. -->
<span data-ttu-id="7238e-107">此 API 提供了通话功能，还可用于创建和检索联机会议。</span><span class="sxs-lookup"><span data-stu-id="7238e-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="7238e-108">可将服务应用程序（机器人）与此 API 搭配使用，其中机器人可在 VoIP 通话或 Microsoft Teams 会议中充当参与者等等。</span><span class="sxs-lookup"><span data-stu-id="7238e-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="7238e-109">授权</span><span class="sxs-lookup"><span data-stu-id="7238e-109">Authorization</span></span>

<span data-ttu-id="7238e-110">需要以下[权限](https://docs.microsoft.com/zh-CN/graph/permissions-reference#calls-permissions) 之一才能访问通信 API。</span><span class="sxs-lookup"><span data-stu-id="7238e-110">One of the following [permissions](https://docs.microsoft.com/zh-CN/graph/permissions-reference#calls-permissions) is required to access user operations.</span></span> <span data-ttu-id="7238e-111">需要由管理员授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="7238e-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="7238e-112">方案</span><span class="sxs-lookup"><span data-stu-id="7238e-112">Scenario</span></span>                 | <span data-ttu-id="7238e-113">权限</span><span class="sxs-lookup"><span data-stu-id="7238e-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="7238e-114">通话</span><span class="sxs-lookup"><span data-stu-id="7238e-114">Calling Plan</span></span>                 | <span data-ttu-id="7238e-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="7238e-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="7238e-116">会议</span><span class="sxs-lookup"><span data-stu-id="7238e-116">Meetings</span></span>                 | <span data-ttu-id="7238e-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="7238e-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="7238e-118">常见用例</span><span class="sxs-lookup"><span data-stu-id="7238e-118">Common use cases</span></span>

<span data-ttu-id="7238e-119">下表列出了通信 API 的一些常见用例。</span><span class="sxs-lookup"><span data-stu-id="7238e-119">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="7238e-120">用例</span><span class="sxs-lookup"><span data-stu-id="7238e-120">Use cases</span></span>                         | <span data-ttu-id="7238e-121">REST 资源</span><span class="sxs-lookup"><span data-stu-id="7238e-121">REST resources</span></span>                                 | <span data-ttu-id="7238e-122">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7238e-122">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="7238e-123">创建并键入一对一通话和群组通话</span><span class="sxs-lookup"><span data-stu-id="7238e-123">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="7238e-124">通话</span><span class="sxs-lookup"><span data-stu-id="7238e-124">Call</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/call?view=graph-rest-beta)| [<span data-ttu-id="7238e-125">通话方法</span><span class="sxs-lookup"><span data-stu-id="7238e-125">Methods for calls</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/call?view=graph-rest-beta#methods)| 
|<span data-ttu-id="7238e-126">IVR 通话</span><span class="sxs-lookup"><span data-stu-id="7238e-126">IVR calls</span></span>   |     | [<span data-ttu-id="7238e-127">IVR 方法</span><span class="sxs-lookup"><span data-stu-id="7238e-127">Methods for IVR</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta)
| <span data-ttu-id="7238e-128">通话控制（参与者）</span><span class="sxs-lookup"><span data-stu-id="7238e-128">Call controls (participant)</span></span> | [<span data-ttu-id="7238e-129">参与者</span><span class="sxs-lookup"><span data-stu-id="7238e-129">Participant</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/participant?view=graph-rest-beta)   ||
|<span data-ttu-id="7238e-130">会议</span><span class="sxs-lookup"><span data-stu-id="7238e-130">Meetings</span></span>|[<span data-ttu-id="7238e-131">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="7238e-131">onlineMeeting</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/onlinemeeting?view=graph-rest-beta)| [<span data-ttu-id="7238e-132">会议方法</span><span class="sxs-lookup"><span data-stu-id="7238e-132">Methods for meetings</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/onlinemeeting?view=graph-rest-beta#methods)|

## <a name="common-properties"></a><span data-ttu-id="7238e-133">通用属性</span><span class="sxs-lookup"><span data-stu-id="7238e-133">Common properties</span></span>

| <span data-ttu-id="7238e-134">资源</span><span class="sxs-lookup"><span data-stu-id="7238e-134">Resource</span></span>                | <span data-ttu-id="7238e-135">属性</span><span class="sxs-lookup"><span data-stu-id="7238e-135">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="7238e-136">通话</span><span class="sxs-lookup"><span data-stu-id="7238e-136">call</span></span>                               | [<span data-ttu-id="7238e-137">通话属性</span><span class="sxs-lookup"><span data-stu-id="7238e-137">call properties</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/call?view=graph-rest-beta#properties)  |
| <span data-ttu-id="7238e-138">参与者</span><span class="sxs-lookup"><span data-stu-id="7238e-138">Participant</span></span>                         | [<span data-ttu-id="7238e-139">参与者属性</span><span class="sxs-lookup"><span data-stu-id="7238e-139">participant properties</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/participant?view=graph-rest-beta#properties) |
| <span data-ttu-id="7238e-140">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="7238e-140">onlineMeeting</span></span>                            | [<span data-ttu-id="7238e-141">onlineMeeting 属性</span><span class="sxs-lookup"><span data-stu-id="7238e-141">onlineMeeting properties</span></span>](https://docs.microsoft.com/en-us/graph/api/resources/onlinemeeting?view=graph-rest-beta#properties)                     |

## <a name="see-also"></a><span data-ttu-id="7238e-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7238e-142">See also</span></span>

- [<span data-ttu-id="7238e-143">通信 API 示例</span><span class="sxs-lookup"><span data-stu-id="7238e-143">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="7238e-144">通信信号 SDK</span><span class="sxs-lookup"><span data-stu-id="7238e-144">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls/1.0.0-prerelease.494)
- [<span data-ttu-id="7238e-145">通信媒体 SDK</span><span class="sxs-lookup"><span data-stu-id="7238e-145">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media/1.0.0-prerelease.494)
