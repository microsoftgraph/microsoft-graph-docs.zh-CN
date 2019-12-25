---
title: 媒体概述
description: 使你的 bot 能够发送和接收与音频和视频相关的内容。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 2ce3f28fc5fc42c5628d6fddac63c69c430a03fd
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871573"
---
# <a name="media-overview"></a><span data-ttu-id="9e5c6-103">媒体概述</span><span class="sxs-lookup"><span data-stu-id="9e5c6-103">Media overview</span></span>

<span data-ttu-id="9e5c6-104">Microsoft Graph 中的云通信 Api 为您的应用和服务如何通过各种通信相关功能（如呼叫和联机会议）与用户进行交互，从而添加了一个新的维度。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-104">The cloud communications APIs in Microsoft Graph add a new dimension to how your apps and services interact with users through various communications related features, such as calling and online meetings.</span></span> <span data-ttu-id="9e5c6-105">您可以启用您的 bot 以发送和接收与音频和视频相关的内容。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-105">You can enable your bots to send and receive audio- and video-related content.</span></span> <span data-ttu-id="9e5c6-106">通过使用媒体，你可以在你的 bot 和用户之间创建更具交互性的体验。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-106">By making use of media, you can create a more interactive experience between your bots and users.</span></span>

<span data-ttu-id="9e5c6-107">本文将帮助您根据自己的需要，发现哪种媒体承载选项适合您。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-107">This article will help you discover which media hosting option is right for you based on your needs.</span></span>

## <a name="service-hosted-media-remote-hosting"></a><span data-ttu-id="9e5c6-108">服务承载的媒体（远程承载）</span><span class="sxs-lookup"><span data-stu-id="9e5c6-108">Service-hosted media (remote hosting)</span></span>
<span data-ttu-id="9e5c6-109">如果您希望您的 bot 在客户拨打您的公司号码时播放自定义提示，或者要检测电话音、录制短语音剪辑或执行各种交互式语音响应（[IVR](/graph/api/resources/calls-api-ivr-overview)）方案，请考虑使用[服务托管的媒体 api](/graph/api/resources/communications-api-overview)。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-109">If you want your bot to play a custom prompt when a customer dials your business's number, or to detect phone tones, record short voice clips, or perform any of the various Interactive Voice Response ([IVR](/graph/api/resources/calls-api-ivr-overview)) scenarios, consider using the [service-hosted media APIs](/graph/api/resources/communications-api-overview).</span></span>

<span data-ttu-id="9e5c6-110">**如果你的媒体需求更简单，请先浏览此选项**。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-110">**If your media needs are simpler, explore this option first**.</span></span> <span data-ttu-id="9e5c6-111">由于远程卸载了重型媒体处理，因此这是一个较轻重量的解决方案，可让你以更灵活的方式构建你的 bot。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-111">Because the heavy media processing is offloaded remotely, this is a lighter weight solution that allows you to build your bot in a more flexible way.</span></span>

<span data-ttu-id="9e5c6-112">有关演示如何创建使用服务托管媒体的 bot 的示例，请参阅[远程媒体呼叫机器人示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples)。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-112">For an example that shows you how to create a bot that uses service-hosted media, see the [Remote media calling bot samples](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/BetaSamples/RemoteMediaSamples).</span></span>

![远程承载关系图](images/communications-remote-media.PNG)

## <a name="application-hosted-media-local-hosting"></a><span data-ttu-id="9e5c6-114">应用程序承载的媒体（本地托管）</span><span class="sxs-lookup"><span data-stu-id="9e5c6-114">Application-hosted media (local hosting)</span></span>
<span data-ttu-id="9e5c6-115">如果您希望您的 bot 访问客户的音频和视频流，以用于通过自然语言处理服务录制、转录、翻译或看法分析，请考虑在本地托管媒体。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-115">If you want your bot to access a live stream of your customers' audio and video to use for recording, transcribing, translating, or sentiment analysis through a natural language processing service, consider hosting your media locally.</span></span>

><span data-ttu-id="9e5c6-116">**注意：** 您不能录制或以其他方式保留来自您的应用程序访问的呼叫或会议的媒体内容或从该媒体内容派生的数据。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-116">**Note:** You may not record or otherwise persist media content from calls or meetings that your application accesses, or data derived from that media content.</span></span> <span data-ttu-id="9e5c6-117">请确保您符合有关通信的数据保护和机密性的法律和法规。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-117">Make sure you are compliant with the laws and regulations of your area regarding data protection and confidentiality of communications.</span></span> <span data-ttu-id="9e5c6-118">有关详细信息，请参阅[使用条款](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use)并咨询法律顾问。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-118">Please see the [Terms of Use](https://docs.microsoft.com/legal/microsoft-apis/terms-of-use) and consult with your legal counsel for more information.</span></span>

<span data-ttu-id="9e5c6-119">**如果您希望更好地控制媒体，请选择此选项**。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-119">**If you'd like more control over your media, choose this option**.</span></span> <span data-ttu-id="9e5c6-120">你将能够直接访问媒体流，并且可以使用基于视频的屏幕共享。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-120">You'll have direct access to media streams and will be able to make use of video-based screen sharing.</span></span> <span data-ttu-id="9e5c6-121">你将能够生成启用了语音的更复杂的 IVR 方案。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-121">You'll be able to build more sophisticated IVR scenarios that are speech enabled.</span></span> <span data-ttu-id="9e5c6-122">这是一个较重的解决方案，为你提供了对媒体编程方式的最大灵活性。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-122">This is a heavier weight solution that gives you the most flexibility in how you want to program your media.</span></span>

<span data-ttu-id="9e5c6-123">另请参阅应用程序托管媒体 bot 的[要求和注意事项](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/requirements-considerations-application-hosted-media-bots)。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-123">See also the [requirements and considerations](https://docs.microsoft.com/microsoftteams/platform/concepts/calls-and-meetings/requirements-considerations-application-hosted-media-bots) for application-hosted media bots.</span></span>

<span data-ttu-id="9e5c6-124">有关演示如何创建使用应用程序承载的媒体的 bot 的示例，请参阅[本地媒体示例](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/V1.0Samples/LocalMediaSamples)。</span><span class="sxs-lookup"><span data-stu-id="9e5c6-124">For an example that shows you how to create a bot that uses application-hosted media, see the [local media samples](https://github.com/microsoftgraph/microsoft-graph-comms-samples/tree/master/Samples/V1.0Samples/LocalMediaSamples).</span></span>

![本地承载关系图](images/communications-local-media.PNG)

## <a name="see-also"></a><span data-ttu-id="9e5c6-126">另请参阅</span><span class="sxs-lookup"><span data-stu-id="9e5c6-126">See also</span></span>

- [<span data-ttu-id="9e5c6-127">通话权限</span><span class="sxs-lookup"><span data-stu-id="9e5c6-127">Calls permissions</span></span>](/graph/permissions-reference#calls-permissions)
