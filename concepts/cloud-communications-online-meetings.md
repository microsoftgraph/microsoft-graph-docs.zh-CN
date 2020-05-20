---
title: 使用云通信 API 创建或加入联机会议
description: 你可以灵活地创建将来或即时使用的会议
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 22d44c32b6ece847283f2e572eeaf468eaac3dbe
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289639"
---
# <a name="use-the-cloud-communications-api-to-create-or-join-online-meetings"></a><span data-ttu-id="a241b-103">使用云通信 API 创建或加入联机会议</span><span class="sxs-lookup"><span data-stu-id="a241b-103">Use the cloud communications API to create or join online meetings</span></span>

<span data-ttu-id="a241b-104">联机会议提供了指定特定详细信息（如会议主题和所有与会者）的功能。</span><span class="sxs-lookup"><span data-stu-id="a241b-104">Online meetings provide the ability to specify certain details, such as the subject of the meeting, and who all the attendees are.</span></span> <span data-ttu-id="a241b-105">您还可以设置会议开始和结束的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="a241b-105">You can also set the date and time for when the meeting starts and ends.</span></span>

<span data-ttu-id="a241b-106">在线会议提供了创建将来或即时召开会议的灵活性。</span><span class="sxs-lookup"><span data-stu-id="a241b-106">Online meetings provide the flexibility to create a meeting that takes place in the future, or instantaneously.</span></span> <span data-ttu-id="a241b-107">设置在创建后立即启动的会议的功能对于需要立即关注与会者的意外问题和其他事件来说是理想之选。</span><span class="sxs-lookup"><span data-stu-id="a241b-107">The ability to set up a meeting that starts immediately after it is created is ideal for unexpected issues and other incidents that require the immediate attention of the attendees.</span></span>

## <a name="create-an-online-meeting"></a><span data-ttu-id="a241b-108">创建联机会议</span><span class="sxs-lookup"><span data-stu-id="a241b-108">Create an online meeting</span></span>

<span data-ttu-id="a241b-109">创建联机会议时，将接收会议的[坐标](/graph/api/resources/onlinemeeting)。</span><span class="sxs-lookup"><span data-stu-id="a241b-109">When you create an online meeting, you'll receive [coordinates](/graph/api/resources/onlinemeeting) for the meeting.</span></span> <span data-ttu-id="a241b-110">当参与者使用这些会议坐标加入会议时，将会创建一个组呼叫。</span><span class="sxs-lookup"><span data-stu-id="a241b-110">When participants join the meeting using these meeting coordinates, a group call is created.</span></span>

<span data-ttu-id="a241b-111">当所有参与者都离开组呼叫时，组呼叫将结束。</span><span class="sxs-lookup"><span data-stu-id="a241b-111">When all the participants leave the group call, the group call will end.</span></span> <span data-ttu-id="a241b-112">参与者仍可以使用相同的会议坐标在随后重新加入会议，但这将创建另一个组呼叫。</span><span class="sxs-lookup"><span data-stu-id="a241b-112">Participants can still rejoin the meeting afterward using the same meeting coordinates, but this will create another group call.</span></span>

><span data-ttu-id="a241b-113">**注意：** 创建的会议不会显示在日历上。</span><span class="sxs-lookup"><span data-stu-id="a241b-113">**Note:** The created meetings do not appear on calendars.</span></span>

## <a name="join-an-online-meeting"></a><span data-ttu-id="a241b-114">加入联机会议</span><span class="sxs-lookup"><span data-stu-id="a241b-114">Join an online meeting</span></span>
<span data-ttu-id="a241b-115">在创建联机会议之后，用户可以通过以下两种方式加入：</span><span class="sxs-lookup"><span data-stu-id="a241b-115">After an online meeting is created, users can join in two ways:</span></span>

1. <span data-ttu-id="a241b-116">通过浏览器，使用作为[会议坐标](/graph/api/resources/onlinemeeting)一部分返回的**joinWebURL** 。</span><span class="sxs-lookup"><span data-stu-id="a241b-116">Through the browser, using the **joinWebURL** that was returned as part of the [meeting coordinates](/graph/api/resources/onlinemeeting).</span></span>

2. <span data-ttu-id="a241b-117">通过[创建调用 API](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media)，它需要您提供[会议坐标](/graph/api/resources/onlinemeeting)（[organizermeetinginfo](/graph/api/resources/organizermeetinginfo)和[chatInfo](/graph/api/resources/chatinfo)）。</span><span class="sxs-lookup"><span data-stu-id="a241b-117">Through the [create call API](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media), which requires that you provide the [meeting coordinates](/graph/api/resources/onlinemeeting), ([organizermeetinginfo](/graph/api/resources/organizermeetinginfo), and [chatInfo](/graph/api/resources/chatinfo)).</span></span>

## <a name="see-also"></a><span data-ttu-id="a241b-118">另请参阅</span><span class="sxs-lookup"><span data-stu-id="a241b-118">See also</span></span>

- [<span data-ttu-id="a241b-119">联机会议权限</span><span class="sxs-lookup"><span data-stu-id="a241b-119">Online meeting permissions</span></span>](/graph/permissions-reference#online-meetings-permissions)
- [<span data-ttu-id="a241b-120">在 Microsoft Graph 中选择 API 以创建和加入联机会议</span><span class="sxs-lookup"><span data-stu-id="a241b-120">Choose an API in Microsoft Graph to create and join online meetings</span></span>](choose-online-meeting-api.md)
