---
title: 使用云通信 API 创建或加入联机会议
description: 你可以灵活地创建将来或即时举行的会议
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 08d7195f3eb91ba896e8045b4576e46f12aaf795
ms.sourcegitcommit: 3fbc2249b307e8d3a9de18f22ef6911094ca272c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2020
ms.locfileid: "48289349"
---
# <a name="use-the-cloud-communications-api-to-create-or-join-online-meetings"></a><span data-ttu-id="95b49-103">使用云通信 API 创建或加入联机会议</span><span class="sxs-lookup"><span data-stu-id="95b49-103">Use the cloud communications API to create or join online meetings</span></span>

<span data-ttu-id="95b49-104">联机会议提供了指定特定详细信息（如会议主题和所有与会者）的功能。</span><span class="sxs-lookup"><span data-stu-id="95b49-104">Online meetings provide the ability to specify certain details, such as the subject of the meeting, and who all the attendees are.</span></span> <span data-ttu-id="95b49-105">您还可以设置会议开始和结束的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="95b49-105">You can also set the date and time for when the meeting starts and ends.</span></span>

<span data-ttu-id="95b49-106">在线会议提供了创建将来或即时召开会议的灵活性。</span><span class="sxs-lookup"><span data-stu-id="95b49-106">Online meetings provide the flexibility to create a meeting that takes place in the future, or instantaneously.</span></span> <span data-ttu-id="95b49-107">设置在创建后立即启动的会议的功能对于需要立即关注与会者的意外问题和其他事件来说是理想之选。</span><span class="sxs-lookup"><span data-stu-id="95b49-107">The ability to set up a meeting that starts immediately after it is created is ideal for unexpected issues and other incidents that require the immediate attention of the attendees.</span></span>

> <span data-ttu-id="95b49-108">**注释** 这组 Api 可提供与 Microsoft 团队或 Skype 功能的灵活性和更丰富的集成;它不会更新或创建日历中的任何事件。</span><span class="sxs-lookup"><span data-stu-id="95b49-108">**Note** This set of APIs allows the flexibility and richer integration with Microsoft Teams or Skype capabilities; it does not update or create any event in a calendar.</span></span> <span data-ttu-id="95b49-109">若要方便地向 Outlook 日历中添加联机会议，请使用日历 API。</span><span class="sxs-lookup"><span data-stu-id="95b49-109">For a convenient approach to add an online meeting to an Outlook calendar, use the calendar API.</span></span> <span data-ttu-id="95b49-110">有关详细信息，请参阅[在 Microsoft Graph 中选择 API 以创建和加入联机会议](choose-online-meeting-api.md)。</span><span class="sxs-lookup"><span data-stu-id="95b49-110">See [Choose an API in Microsoft Graph to create and join online meetings](choose-online-meeting-api.md) for more information.</span></span>

## <a name="create-an-online-meeting"></a><span data-ttu-id="95b49-111">创建联机会议</span><span class="sxs-lookup"><span data-stu-id="95b49-111">Create an online meeting</span></span>

<span data-ttu-id="95b49-112">创建联机会议时，将接收会议的 [坐标](/graph/api/resources/onlinemeeting) 。</span><span class="sxs-lookup"><span data-stu-id="95b49-112">When you create an online meeting, you'll receive [coordinates](/graph/api/resources/onlinemeeting) for the meeting.</span></span> <span data-ttu-id="95b49-113">当参与者使用这些会议坐标加入会议时，将会创建一个组呼叫。</span><span class="sxs-lookup"><span data-stu-id="95b49-113">When participants join the meeting using these meeting coordinates, a group call is created.</span></span>

<span data-ttu-id="95b49-114">当所有参与者都离开组呼叫时，组呼叫将结束。</span><span class="sxs-lookup"><span data-stu-id="95b49-114">When all the participants leave the group call, the group call will end.</span></span> <span data-ttu-id="95b49-115">参与者仍可以使用相同的会议坐标在随后重新加入会议，但这将创建另一个组呼叫。</span><span class="sxs-lookup"><span data-stu-id="95b49-115">Participants can still rejoin the meeting afterward using the same meeting coordinates, but this will create another group call.</span></span>

><span data-ttu-id="95b49-116">**注意：** 创建的会议不会显示在日历上。</span><span class="sxs-lookup"><span data-stu-id="95b49-116">**Note:** The created meetings do not appear on calendars.</span></span>

## <a name="join-an-online-meeting"></a><span data-ttu-id="95b49-117">加入联机会议</span><span class="sxs-lookup"><span data-stu-id="95b49-117">Join an online meeting</span></span>
<span data-ttu-id="95b49-118">在创建联机会议之后，用户可以通过以下两种方式加入：</span><span class="sxs-lookup"><span data-stu-id="95b49-118">After an online meeting is created, users can join in two ways:</span></span>

1. <span data-ttu-id="95b49-119">通过浏览器，使用作为[会议坐标](/graph/api/resources/onlinemeeting)一部分返回的**joinWebURL** 。</span><span class="sxs-lookup"><span data-stu-id="95b49-119">Through the browser, using the **joinWebURL** that was returned as part of the [meeting coordinates](/graph/api/resources/onlinemeeting).</span></span>

2. <span data-ttu-id="95b49-120">通过 [创建调用 API](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media)，它需要您提供 [会议坐标](/graph/api/resources/onlinemeeting)、 ([organizermeetinginfo](/graph/api/resources/organizermeetinginfo)和 [chatInfo](/graph/api/resources/chatinfo)) 。</span><span class="sxs-lookup"><span data-stu-id="95b49-120">Through the [create call API](/graph/api/application-post-calls#example-5-join-scheduled-meeting-with-service-hosted-media), which requires that you provide the [meeting coordinates](/graph/api/resources/onlinemeeting), ([organizermeetinginfo](/graph/api/resources/organizermeetinginfo), and [chatInfo](/graph/api/resources/chatinfo)).</span></span>

## <a name="see-also"></a><span data-ttu-id="95b49-121">另请参阅</span><span class="sxs-lookup"><span data-stu-id="95b49-121">See also</span></span>

- [<span data-ttu-id="95b49-122">联机会议权限</span><span class="sxs-lookup"><span data-stu-id="95b49-122">Online meeting permissions</span></span>](./permissions-reference.md#online-meetings-permissions)
- [<span data-ttu-id="95b49-123">在 Microsoft Graph 中选择 API 以创建和加入联机会议</span><span class="sxs-lookup"><span data-stu-id="95b49-123">Choose an API in Microsoft Graph to create and join online meetings</span></span>](choose-online-meeting-api.md)