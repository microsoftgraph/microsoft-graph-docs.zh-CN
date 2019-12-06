---
title: 使用 Microsoft Graph 通信 API
description: Microsoft Graph 通信 API 通过启用语音和视频功能，为应用和服务与用户的互动方式添加了新的维度。
author: VinodRavichandran
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 99f79861ae4641f29784ebad44c14408a69821d9
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39843936"
---
# <a name="working-with-the-communications-api-in-microsoft-graph"></a><span data-ttu-id="78adb-103">使用 Microsoft Graph 通信 API</span><span class="sxs-lookup"><span data-stu-id="78adb-103">Working with the communications API in Microsoft Graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78adb-104">Microsoft Graph 通信 API 通过在应用和服务中启用核心通信功能，为你或你的组织与其他用户交互的方式添加了新的维度。</span><span class="sxs-lookup"><span data-stu-id="78adb-104">The Microsoft Graph communications API adds a new dimension to how you or your organization can interact with other users by enabling core communication capabilities and features in your apps and services.</span></span> <span data-ttu-id="78adb-105">可使用此 API 接听电话、创建和检索会议坐标和查看用户的状态。</span><span class="sxs-lookup"><span data-stu-id="78adb-105">You can use this API to create and receive calls, create and retrieve meeting coordinates, and check users' presence.</span></span>

<span data-ttu-id="78adb-106">可使用通信 API 构建服务应用程序（机器人），它们在通话中充当参与者，代表用户创建和检索会议并检查出席状态和活动。</span><span class="sxs-lookup"><span data-stu-id="78adb-106">You can use the communications API to build service applications (bots) that act like participants in a call, and that create and retrieve meetings on behalf of users.</span></span>
<span data-ttu-id="78adb-107">此 API 提供了通话功能，还可用于创建和检索联机会议。</span><span class="sxs-lookup"><span data-stu-id="78adb-107">This API provides calling functionality as well as the ability to create and retrieve online meetings.</span></span> <span data-ttu-id="78adb-108">可将服务应用程序（机器人）与此 API 搭配使用，其中机器人可在 VoIP 通话或 Microsoft Teams 会议中充当参与者等等。</span><span class="sxs-lookup"><span data-stu-id="78adb-108">You can use service applications (bots) with this API, where the bot can act as a participant in your VoIP calls or Microsoft Teams meetings, for example.</span></span>

## <a name="authorization"></a><span data-ttu-id="78adb-109">授权</span><span class="sxs-lookup"><span data-stu-id="78adb-109">Authorization</span></span>

<span data-ttu-id="78adb-110">需要以下[权限](https://docs.microsoft.com/graph/permissions-reference#calls-permissions) 之一才能访问通信 API。</span><span class="sxs-lookup"><span data-stu-id="78adb-110">One of the following [permissions](https://docs.microsoft.com/graph/permissions-reference#calls-permissions) is required to access the communications API.</span></span> <span data-ttu-id="78adb-111">需要由管理员授予这些权限。</span><span class="sxs-lookup"><span data-stu-id="78adb-111">These permissions need to be granted by the administrator</span></span>

| <span data-ttu-id="78adb-112">方案</span><span class="sxs-lookup"><span data-stu-id="78adb-112">Scenario</span></span>                 | <span data-ttu-id="78adb-113">权限</span><span class="sxs-lookup"><span data-stu-id="78adb-113">Permissions</span></span>                                  |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="78adb-114">通话</span><span class="sxs-lookup"><span data-stu-id="78adb-114">Calling</span></span>                 | <span data-ttu-id="78adb-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span><span class="sxs-lookup"><span data-stu-id="78adb-115">Calls.JoinGroupCallsasGuest.All, Calls.JoinGroupCalls.All, Calls.Initiate.All, Calls.InitiateGroupCalls.All, Calls.AccessMedia.All</span></span> |
| <span data-ttu-id="78adb-116">会议</span><span class="sxs-lookup"><span data-stu-id="78adb-116">Meetings</span></span>                 | <span data-ttu-id="78adb-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span><span class="sxs-lookup"><span data-stu-id="78adb-117">OnlineMeetings.ReadWrite.All, OnlineMeetings.Read.All</span></span> |
| <span data-ttu-id="78adb-118">状态</span><span class="sxs-lookup"><span data-stu-id="78adb-118">Presence</span></span>                 | <span data-ttu-id="78adb-119">状态.阅读，状态.阅读.全部</span><span class="sxs-lookup"><span data-stu-id="78adb-119">Presence.Read, Presence.Read.All</span></span> |

## <a name="common-use-cases"></a><span data-ttu-id="78adb-120">常见用例</span><span class="sxs-lookup"><span data-stu-id="78adb-120">Common use cases</span></span>

<span data-ttu-id="78adb-121">下表列出了通信 API 的一些常见用例。</span><span class="sxs-lookup"><span data-stu-id="78adb-121">The following table lists some of the common uses for the communications API.</span></span>

| <span data-ttu-id="78adb-122">用例</span><span class="sxs-lookup"><span data-stu-id="78adb-122">Use cases</span></span>                         | <span data-ttu-id="78adb-123">REST 资源</span><span class="sxs-lookup"><span data-stu-id="78adb-123">REST resources</span></span>                                 | <span data-ttu-id="78adb-124">另请参阅</span><span class="sxs-lookup"><span data-stu-id="78adb-124">See also</span></span>  |
|:------------------------------------|:---------------------------------------------|:----------|
| <span data-ttu-id="78adb-125">创建并键入一对一通话和群组通话</span><span class="sxs-lookup"><span data-stu-id="78adb-125">Creating and joining 1-1 and group calls</span></span>   | [<span data-ttu-id="78adb-126">通话</span><span class="sxs-lookup"><span data-stu-id="78adb-126">Call</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-beta)| [<span data-ttu-id="78adb-127">通话方法</span><span class="sxs-lookup"><span data-stu-id="78adb-127">Methods for calls</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-beta#methods)| 
|<span data-ttu-id="78adb-128">IVR 通话</span><span class="sxs-lookup"><span data-stu-id="78adb-128">IVR calls</span></span>   |     | [<span data-ttu-id="78adb-129">IVR 方法</span><span class="sxs-lookup"><span data-stu-id="78adb-129">Methods for IVR</span></span>](https://docs.microsoft.com/graph/api/resources/calls-api-ivr-overview?view=graph-rest-beta)
| <span data-ttu-id="78adb-130">通话控制（参与者）</span><span class="sxs-lookup"><span data-stu-id="78adb-130">Call controls (participant)</span></span> | [<span data-ttu-id="78adb-131">参与者</span><span class="sxs-lookup"><span data-stu-id="78adb-131">Participant</span></span>](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-beta)   ||
|<span data-ttu-id="78adb-132">会议</span><span class="sxs-lookup"><span data-stu-id="78adb-132">Meetings</span></span>|[<span data-ttu-id="78adb-133">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="78adb-133">onlineMeeting</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-beta)| [<span data-ttu-id="78adb-134">会议方法</span><span class="sxs-lookup"><span data-stu-id="78adb-134">Methods for meetings</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-beta#methods)|
|<span data-ttu-id="78adb-135">状态</span><span class="sxs-lookup"><span data-stu-id="78adb-135">Presence</span></span> | [<span data-ttu-id="78adb-136">状态</span><span class="sxs-lookup"><span data-stu-id="78adb-136">Presence</span></span>](/graph/api/resources/presence) | [<span data-ttu-id="78adb-137">出席方式</span><span class="sxs-lookup"><span data-stu-id="78adb-137">Methods for presence</span></span>](/graph/api/resources/presence#methods) |

## <a name="common-properties"></a><span data-ttu-id="78adb-138">通用属性</span><span class="sxs-lookup"><span data-stu-id="78adb-138">Common properties</span></span>

| <span data-ttu-id="78adb-139">资源</span><span class="sxs-lookup"><span data-stu-id="78adb-139">Resource</span></span>                | <span data-ttu-id="78adb-140">属性</span><span class="sxs-lookup"><span data-stu-id="78adb-140">Properties</span></span>                             |
|:------------------------------------|:---------------------------------------------|
| <span data-ttu-id="78adb-141">通话</span><span class="sxs-lookup"><span data-stu-id="78adb-141">call</span></span>                               | [<span data-ttu-id="78adb-142">通话属性</span><span class="sxs-lookup"><span data-stu-id="78adb-142">call properties</span></span>](https://docs.microsoft.com/graph/api/resources/call?view=graph-rest-beta#properties)  |
| <span data-ttu-id="78adb-143">参与者</span><span class="sxs-lookup"><span data-stu-id="78adb-143">participant</span></span>                         | [<span data-ttu-id="78adb-144">参与者属性</span><span class="sxs-lookup"><span data-stu-id="78adb-144">participant properties</span></span>](https://docs.microsoft.com/graph/api/resources/participant?view=graph-rest-beta#properties) |
| <span data-ttu-id="78adb-145">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="78adb-145">onlineMeeting</span></span>                            | [<span data-ttu-id="78adb-146">onlineMeeting 属性</span><span class="sxs-lookup"><span data-stu-id="78adb-146">onlineMeeting properties</span></span>](https://docs.microsoft.com/graph/api/resources/onlinemeeting?view=graph-rest-beta#properties)                     |
| <span data-ttu-id="78adb-147">状态</span><span class="sxs-lookup"><span data-stu-id="78adb-147">Presence</span></span> | [<span data-ttu-id="78adb-148">状态属性</span><span class="sxs-lookup"><span data-stu-id="78adb-148">presence properties</span></span>](/graph/api/resources/presence#properties) |

## <a name="see-also"></a><span data-ttu-id="78adb-149">另请参阅</span><span class="sxs-lookup"><span data-stu-id="78adb-149">See also</span></span>

- [<span data-ttu-id="78adb-150">通信 API 示例</span><span class="sxs-lookup"><span data-stu-id="78adb-150">Communications API samples</span></span>](https://github.com/microsoftgraph/microsoft-graph-comms-samples/)
- [<span data-ttu-id="78adb-151">通信信号 SDK</span><span class="sxs-lookup"><span data-stu-id="78adb-151">Communication Signaling SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls/1.0.0-prerelease.494)
- [<span data-ttu-id="78adb-152">通信媒体 SDK</span><span class="sxs-lookup"><span data-stu-id="78adb-152">Communication Media SDK</span></span>](https://www.nuget.org/packages/Microsoft.Graph.Communications.Calls.Media/1.0.0-prerelease.494)
